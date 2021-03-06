实验四
======

提交截止时间为7月2日晚23:00，请注意GitHub将在截止时间到达时锁定你的仓库，不再接受变更。

请大家通过此链接在GitHub上提交[实验四](https://classroom.github.com/a/6DCVURgC)。


实验目的
--------

本实验旨在综合所学内容，了解处理器漏洞[Meltdown](https://meltdownattack.com/)和[Spectre](https://spectreattack.com/)，掌握基本的漏洞分析和攻击方法，提升资料查找和文献阅读能力。


实验要求
--------

从Meltdown（难度较低）和Spectre（难度较高）的变种中任选一种，仔细阅读对应的论文，并查阅相关资料，了解漏洞的背景、原理，以及漏洞可能的利用方式，并利用漏洞编写一个完整的攻击程序，实现越权内存访问。

请同时提交一份实验报告，说明你的程序的原理、攻击步骤、期望的结果。另外建议提交编译脚本或项目文件（CMakeList.txt/Makefile/yourproject.vcxproj等）并说明测试环境。

另请特别注意：在你的实验报告中如有使用其他文献中的介绍，请在报告中正确地进行引用；在你的程序中如有使用其他人的代码（包括论文中的代码），请在源文件中正确地进行声明，否则一律视为抄袭行为。


关于Makefile
------------

一个最简单的Makefile文件如下：

```make
default:
	gcc -o program.exe source.c
```

将其保存为一个名为Makefile的文件，之后便可以直接通过标准的`make`命令编译你的程序。学会使用Makefile等自动构建工具可以让他人更加快速的运行你的代码。对于更大型的项目，还可以进一步采用autotools或cmake等工具自动化地生成Makefile。


关于实验环境
------------

由于最新的系统均部署了针对此系列漏洞的更新，请使用老版本的系统进行实验，如未开启自动更新的Windows 10 1709或Linux Kernel 4.14以前的操作系统。另请注意，由于本系列漏洞属于cpu设计上的缺陷，而非操作系统本身的漏洞，因此在宿主机上使用新版本操作系统也可能对虚拟机内操作系统产生一部分影响。
