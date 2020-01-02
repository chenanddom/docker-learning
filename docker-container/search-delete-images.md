# 查看镜像和删除镜像

## 列出镜像

docker images [OPTIONS] [REPOSITORY]
 -a,--all=false 列出所有镜像,默认不显示中间层的镜像
 -f,--filter=[] 过滤镜像
 --no-trunc=false 默认使用截断的形式
 -q --quiet=false 只现实镜像的唯一id
 
 
## 镜像仓库

* REPOSITORY 仓库(存放一个个镜像的仓库)

* REGISTRY 仓库(包含了多个Repository)



## 镜像的标签
* TAG



## 删除镜像

docker rmi [OPTIONS] IMAGE [IMAGE....]
-f,--force=false 强制删除镜像
--no-prune=false 保留被打标签的父镜像
