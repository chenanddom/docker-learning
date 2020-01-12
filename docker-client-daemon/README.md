#Docker的C/S模式

![Docker的C/S模式](images/docker-16.png)


## Remote API

* RESTful风格的API
* 支持STDIN,STDOUT,STDERR

![Remote API](images/docker-17.png)


## Docker 的C/S模式的连接方式

* unix:///var/run/docker.sock(默认的)

* tcp://host:port

* fd://socketfd

例子:

![Remote API](images/docker-18.png)