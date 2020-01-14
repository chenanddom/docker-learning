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





