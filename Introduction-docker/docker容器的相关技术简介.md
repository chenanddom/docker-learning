#Docker容器相关技术简介

## docker依赖Linux内核特性

* NameSpaces 命名空间
    提供了系统字眼的隔离(进程，网络，文件系统...)

    1. PID(Process ID) 进程隔离
    2. NET (Network) 管理网接口
    3. IPC(InterProcess Communication) 管理跨进程通信的访问
    4. MNT(Mount) 管理挂载点
    5. UTS (Unix Timesharing System) 隔离内核和版本标识
    
    
    
    

* Control group (cgroup)控制组

 1. 用来分配资源
    1.资源限制
    2.有限级设定
    3.资源计量
    4.资源控制
 
 2. 来源于google
 3. 2007年诞生

## Docker 容器的能力

* 文件系统隔离：每个容器都有自己的root文件系统
* 进程隔离:每个容器都运行在自己的进程环境中
* 网络隔离：容器间 的网络接口和IP地址都是分开的
* 资源隔离和分组: 使用cgroups和CPU和内存之类的资源独立的分配给每个Docker容器













