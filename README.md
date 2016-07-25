# 1.编译x264
1.1在编译x264之前编译yasm

	./configure
	make && make install
yasm简介

&emsp;Yasm是一个完全重写的NASM汇编。目前，它支持x86和AMD64指令集，接受NASM和气体汇编语法，产出二进制， ELF32 ， ELF64 ， COFF ， Mach - O的（ 32和64 ） ， RDOFF2 ，的Win32和Win64对象的格式，并生成STABS 调试信息的来源，DWARF 2 ，CodeView 8格式。

1.2.编译x264

	./configure
	make && make install


