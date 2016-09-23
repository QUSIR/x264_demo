# 1.编译x264
1.1在编译x264之前编译yasm

	./configure
	make && make install
yasm简介

&emsp;Yasm是一个完全重写的NASM汇编。目前，它支持x86和AMD64指令集，接受NASM和气体汇编语法，产出二进制， ELF32 ， ELF64 ， COFF ， Mach - O的（ 32和64 ） ， RDOFF2 ，的Win32和Win64对象的格式，并生成STABS 调试信息的来源，DWARF 2 ，CodeView 8格式。

1.2.编译x264

	./configure
	make && make install
1.3.交叉编译

	./configure --host=arm-linux --prefix=/usr/local/x264-arm --enable-shared --enable-debug --disable-asm

修改配置文件



	vi config.mak



 



把里面的的


	cc=gcc 改成cc=arm-linux-gcc

	ar=ar 改成ar=arm-linux-ar

	ranlib=ranlib 改成 ranlib=arm-linux-ranlib

	LD=gcc -o 改成LD=arm-linux-gcc -o 

#程序样例
在目录`test`下，编译成功的平台在X86，ARM平台下编译不成功，Android平台还没试。