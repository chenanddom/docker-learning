# Dockerfile指令--指令格式


# Comment
INSTRUCTION argument






## 指令类型

* FROM

1. FROM <image>(必须已经存在的镜像，必须是第一条非注释的指令)
2. FROM <image>:<tag>


* MAINTAINER

指定镜像的作者信息，包含镜像的所有者和联系信息






* RUN

在docker镜像上运行的命令

* EXPOSE
指定暴露的端口
EXPOSE<port>[<port>...]，但是docker并不会自动的打开端口，而实在执行镜像的时候加上端口

docker run -p 80 -d dormancypress/docker_file_test nginx -g "daemon off"



## 容器运行时的命令

* CMD

CMD ["executable","param1","param2"](exec模式)

CMD command param1 param2(shell 模式)

CMD ["param1","param2"](作为ENTRYPOINT指令的默认参数)


注意：run 命令指定的命令会覆盖docker file 的CMD命令




* ENTERYPOINT


## 设置镜像的目录和文件

* ADD

该指令包含了类似tar的解压功能

* COPY
如果单纯复制文件，Docker推荐使用COPY



* VOLUME

可以绕过联合文件系统，实现文件系统的共享


## 镜像构建和容器运行的时的环境设置


* WORKDIR

镜像创建新容器时，指定工作目录，WORKDIR使用的时绝对路径，如果使用了相对路径会一直传递下去
例如：

WORDKDIR /a
WORKDIR b
WORKDIR c

---->/a/b/c



* ENV


设置环境变量，在构建镜像和运行镜像都生效





* USER
指定镜像是说明用户运行(默认使用root用户)
例如 USER nginx



## 触发器

* ONBUILD

镜像触发器
使用场景：当一个镜像被其他的镜像作为基础镜像时时执行
会在构建过程中插入指令
















