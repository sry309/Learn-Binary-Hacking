gcc 
================================

- ``-c`` 只执行预处理、编译、汇编，不执行链接过程
- ``-m32`` 生成32bit程序需要gcc-multilib(x86机器上编译不用加)
- ``-Ox`` 设置优化的等级
- ``-o`` 生成的文件名
- ``-fno-stack-protector`` 不开启canary栈溢出检测
- ``-z execstack`` 开启栈可执行关闭NX
- ``-E`` 输出预处理文件
- ``-S`` 输出汇编文件
