# Docker容器的基本操作

##启动容器

docker run IMAGE [COMMAND] [ARG...]


## 启动交互式容器

docker run -i -t IMAGE /bin/bash
  -i --interactive=true|false 默认时false(告诉docker开启标准输入)
  -t --tty=true|false 默认是false(告诉docker容器开启一个伪终端tty)

## 查看容器
 docker ps [-a][-l]
  -a :列出所有的容器
  -l:列出最新创建的容器

 docker inspect :查看容器的详细信息






