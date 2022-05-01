# 部署环境

OS: Ubuntu 16.04



# 修改部分文件

## Linux编译Peach文件的过程中 

修改aflsmart/peach-3.0.202-source/3rdParty/pin/pin-2.12-54730-gcc.4.4.7-linux/source/include/compiler_version_check2.H

主要修改了：
1. 删除了.H文件头部error报错部分

## 修改setup_env.sh文件

将文件中首句SCRIPT=$(readlink -f "$0")改为SCRIPT=$(readlink -f -- "$0")，否则Ubuntu系统不会通过。

## 分析aflsmart/WavPack/out/crashes中crash文件

分析崩溃文件中具体崩溃，参考后续分析工程。

