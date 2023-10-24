如果这是你第一次使用 Django 的话，你需要一些初始化设置。也就是说，你需要用一些自动生成的代码配置一个 Django project -- 即一个 Django 项目实例需要的设置项集合，包括数据库配置、Django 配置和应用程序配置。
打开命令行，`cd` 到一个你想放置你代码的目录，然后运行以下命令：
```bash
$ django-admin startproject mysite
```
这行代码将会在当前目录下创建一个 **mysite** 目录。
Let's look at what startproject created:
```bash
mysite/
    manage.py
    mysite/
        __init__.py
        settings.py
        urls.py
        asgi.py
        wsgi.py
```
这些目录和文件的用处是：

- 最外层的 **mysite/** 根目录只是你项目的容器， 根目录名称对 Django 没有影响，你可以将它重命名为任何你喜欢的名称。
- `manage.py`: 一个让你用各种方式管理 Django 项目的命令行工具。
- 里面一层的 **mysite/** 目录包含你的项目，它是一个纯 Python 包。它的名字就是当你引用它内部任何东西时需要用到的 Python 包名。 (比如 **mysite.urls**).
- `mysite/__init__.py`：一个空文件，告诉 Python 这个目录应该被认为是一个 Python 包。
- `mysite/settings.py`：Django 项目的配置文件。
- `mysite/urls.py`：Django 项目的 URL 声明，就像你网站的“目录”。
- `mysite/asgi.py`：作为你的项目的运行在 ASGI 兼容的 Web 服务器上的入口。
- `mysite/wsgi.py`：作为你的项目的运行在 WSGI 兼容的Web服务器上的入口。