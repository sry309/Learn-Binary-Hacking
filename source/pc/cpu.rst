CPU
====================================

指令集架构
------------------------------------

简介
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
指令集架构（英语：Instruction Set Architecture，缩写为ISA），又称指令集或指令集体系，是计算机体系结构中与程序设计有关的部分，包含了基本数据类型、指令集、寄存器、寻址模式、存储体系、中断、异常处理以及外部I/O。指令集架构包含一系列的opcode即操作码（机器语言），以及由特定处理器执行的基本命令。

指令集体系与微架构（一套用于执行指令集的微处理器设计方法）不同。使用不同微架构的计算机可以共享一种指令集。例如，Intel的Pentium和AMD的AMD Athlon，两者几乎采用相同版本的x86指令集体系，但是两者在内部设计上有本质的区别。 

分类
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
指令集分为复杂指令集（Complex Instruction Set Computing，CISC）和精简指令集（Reduced Instruction Set Computing，RISC）。

复杂指令集计算机包含许多应用程序中很少使用的特定指令，由此产生的缺陷是指令长度不固定。精简指令集计算机通过只执行在程序中经常使用的指令来简化处理器的结构，而特殊操作则以子程序的方式实现，它们的特殊使用通过处理器额外的执行时间来弥补。

x86架构
------------------------------------

寄存器
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
- ESP
    - Extended Stack Pointer 栈指针寄存器
    - 指向最上面帧的栈顶
- EBP
    - Extended Base Pointer 基址指针寄存器
    - 指向最上面帧的栈底
- EIP
    - Extended Instruction Pointer 指令寄存器
    - 指向当前的指令地址
- EFLAGS
    - 保存当前执行状态的所有Flag
- CR0-CR7
    - 控制寄存器
    - 保存系统的控制位
- IDTR
    - Interrupt Descriptor Table Register
    - 中断寄存器，记录当前中断处理函数的地址
- IDTR
    - Global Descriptor Table Register
    - 记录段表

权限
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
ring0到ring3，ring0为最高权限，ring3最低，一般ring0为内核权限，ring3为用户权限，很少用ring1和ring2。

参考链接
------------------------------------
- `List of Intel microprocessors <https://en.wikipedia.org/wiki/List_of_Intel_microprocessors>`_
- `List of ARM microarchitectures <https://en.wikipedia.org/wiki/List_of_ARM_microarchitectures>`_
- `List of AMD microprocessors <https://en.wikipedia.org/wiki/List_of_AMD_microprocessors>`_
