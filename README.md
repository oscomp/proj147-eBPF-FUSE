# proj147-eBPF-FUSE
基于eBPF实现高性能用户态文件系统功能


### 支持单位
DatenLord

### 项目描述
eBPF是Linux内核的新特性，方便用户在内核里安全运行自定义的逻辑，eBPF在网络、安全、可观测性方面已经有了很多应用，但是在文件IO方面的工作还不多。

Filesystem in User-SpacE(FUSE)是Linux内核的用户态文件系统接口，方便用户实现用户态文件系统并与Linux内核对接。FUSE接口目前有很大的性能瓶颈，由于FUSE在用户态和内核态之间的数据传输要做内存拷贝。

本项目要求是基于eBPF实现用户态文件系统功能，同时要求保证高性能，即在用户态和内核态之间传输数据时避免内存拷贝。

### 所属赛道

2022全国大学生操作系统比赛的“OS功能挑战”赛道

### 参赛要求

- 熟悉eBPF
- 熟悉Rust，特别是Rust异步编程

### 项目导师

郑昱笙

* github ：https://github.com/yunwei37
* email：yunwei356@gmail.com and team@eunomia.dev

### 难度

高难度

### 特征

- 建议基于Linux内核5.10以上版本
- BPF的程序可以采用C或Rust实现
- 用户态文件系统的功能建议采用Rust实现

### License
- GPL-2.0 License

## 预期目标

- 基于eBPF实现高性能FUSE接口，支持在用户态和内核态之间共享数据，并且避免内存拷贝
- 基于eBPF实现的FUSE接口，实现用户态文件系统功能，至少要求实现文件增删改查功能


