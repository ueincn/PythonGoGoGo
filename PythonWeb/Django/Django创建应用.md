Django 中，每一个应用都是一个 Python 包，并且遵循着相同的约定。Django 自带一个工具，可以帮你生成应用的基础目录结构，这样你就能专心写代码，而不是创建目录了。你的应用可以存放在任何 Python 路径中定义的路径。
```bash
python manage.py startapp polls
```
That'll create a directory **polls**, which is laid out like this:
```bash
polls/
    __init__.py
    admin.py
    apps.py
    migrations/
        __init__.py
    models.py
    tests.py
    views.py
```