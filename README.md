# 使用帮助 #

本Docker镜像用于Ruby的开发环境，使用```Ruby 2.2.3```版本。

## 创建镜像 ##

```
$ git clone https://github.com/gaoermai/docker-ruby-devel.git
$ cd docker-ruby-devel/
$ docker build -t <your_name>/ruby-devel:0.0.2 .
```

## 创建开发用容器 ##

创建镜像：

```
$ docker run -tid -p 3000:3000 -v /path/to/your/code:/data --name <your_container_name> <your_name>/ruby-devel:0.0.2
```

进入已运行的镜像：

```
$ docker exec -it <your_container_name> /bin/bash
```