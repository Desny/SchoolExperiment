# SchoolExperiment

###操作系统实验：处理机调度算法的实现  （此算法是用C语言实现的）

实验内容：

1．设定系统中有五个进程，每一个进程用一个进程控制块表示。

2．输入每个进程的“优先数”和“要求运行时间”。

3．为了调度方便，将五个进程按给定的优先数从大到小连成就绪队列。用一单元指出队列首进程，用指针指出队列的连接情况。

4．处理机调度总是选队首进程运行。采用动态优先数算法，进程每运行一次优先数就减“1”，同时将运行时间减“1”。

5．若某进程运行时间为零，则将其状态置为“结束”,且退出队列。

运行所设计程序，显示或打印逐次被选中进程的进程名，以及进程控制块的动态变化过程。

实验仍然存在的 2 个问题：代码仍然存在一定量的冗余；虽然已经尽可能做到减少系统资源的开销，但不能确定是否依然产生了大量的malloc未free


###操作系统实验：存储器的分配与回收算法实现  （此算法是用C语言实现的）

实验内容：

1. 模拟操作系统的主存分配，运用可变分区的存储管理算法设计主存分配和回收程序，并不实际启动装入作业。

2. 采用最先适应法、最佳适应法、最坏适应法分配主存空间。

3. 当一个新作业要求装入主存时，必须查空闲区表，从中找出一个足够大的空闲区。若找到的空闲区大于作业需要量，这是应把它分成二部分，一部分为占用区，加一部分又成为一个空闲区。

4. 当一个作业撤离时，归还的区域如果与其他空闲区相邻，则应合并成一个较大的空闲区，登在空闲区表中。

5. 运行所设计的程序，输出有关数据结构表项的变化和内存的当前状态。

我这个实验的代码有一些关于双向链表的插入是没必要的，做完实验才发现的，但是我还是一并传上来。这次主要学会了减少纸上的设计思路的书写，而是用空函数的方式搭建出大体框架，然后再慢慢填充。每填充1~2个函数还要test一下，及早发现错误。这个实验的部分代码存在冗余现象，以后再注意吧……

###操作系统实验：磁盘调度算法的实现  （此算法是用C语言实现的）

实验内容：

1．本实验是模拟操作系统的磁盘寻道方式，运用磁盘访问顺序的不同来设计磁盘的调度算法。

2．实现的磁盘调度算法有FCFS，SSTF，SCAN，CSCAN和 NStepSCAN算法。

3．设定开始磁道号寻道范围，依据起始扫描磁道号和最大磁道号数，随机产生要进行寻道的磁道号序列。

4．选择磁盘调度算法，显示该算法的磁道访问顺序，计算出移动的磁道总数和平均寻道总数。

5．按算法的寻道效率进行排序，并对各算法的性能进行分析比较。

这个实验写的充满作业性质啊，我个人觉得函数的设计上马马虎虎的，虽然结果对了，但是逻辑上有点混乱= =但是作业嘛，你懂得~以后自己要编个软件的话会很认真哒~
那一天赶紧来吧~

