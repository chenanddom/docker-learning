# Docker 容器互联
## Docker容器的互联--允许所有的容器间互联
~~~
--icc=true 默认

~~~
~~~
--link
docker run --link=[CONTAINER_NAME]:[ALIAS] [IMAGE] [COMMAND]

~~~

## Docker容器的互联--拒绝所有容器的访问
我这里需要在/etc/docker/daemon.json添加该选项
~~~
--icc=false
~~~

## 允许特定容器间的连接

~~~
--icc=false --iptable=true
--link


~~~