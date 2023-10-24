#### 启动用于开发的简易服务器
```bash
$ python manage.py runserver
#默认情况下，runserver 命令会将服务器设置为监听本机内部 IP 的 8000 端口。
#下面的命令会使服务器监听 8080 端口
$ python manage.py runserver 8080
#监听所有服务器的公开IP
$ python manage.py runserver 0.0.0.0:8000
```
#### 创建数据库
```bash
#Python 内置 SQLite，所以你无需安装额外东西来使用它。
$ python manage.py migrate
```