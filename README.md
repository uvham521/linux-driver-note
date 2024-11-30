# Linux 驱动笔记

记录学习 Linux 驱动时写下的代码示例。

## 准备

我使用的是 ROC-RK3328-CC 开发板，运行的系统是 Armbian - Ubuntu 24.04 (Noble) Server 版本。

- https://www.armbian.com/renegade/
- Build Date: Nov 25, 2024

在启动系统之后，需要安装 linux headers 包，方法是执行 `sudo armbian-config` 找到 System -> Install Linux headers，安装完重启系统即可。

## 驱动示例

我把写过的驱动示例列举如下：
1. 简单的 HelloWorld 驱动模块

## 参考资料

- [Johannes 4GNU_Linux - Let's code a Linux Driver](https://www.youtube.com/playlist?list=PLCGpd0Do5-I3b5TtyqeF1UdyD4C-S-dMa)
- [北京迅为 - 嵌入式学习之Linux驱动](https://www.bilibili.com/video/BV1vg411S7QW)
