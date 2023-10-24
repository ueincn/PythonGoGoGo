## Django安装
#### pip安装
```bash
pip install Django

#安装指定版本
pip install Django== 4.2.6
```
示例：
```bash
(venv) PS D:\DevSpace\Python\Project\djangoweb> pip install Django
Collecting Django
  Downloading Django-4.2-py3-none-any.whl (8.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 8.0/8.0 MB 169.9 kB/s eta 0:00:00
Collecting asgiref<4,>=3.6.0
  Downloading asgiref-3.6.0-py3-none-any.whl (23 kB)
Collecting sqlparse>=0.3.1
  Downloading sqlparse-0.4.4-py3-none-any.whl (41 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 41.2/41.2 kB 219.5 kB/s eta 0:00:00
Collecting tzdata
  Downloading tzdata-2023.3-py2.py3-none-any.whl (341 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 341.8/341.8 kB 114.7 kB/s eta 0:00:00
Installing collected packages: tzdata, sqlparse, asgiref, Django
Successfully installed Django-4.2 asgiref-3.6.0 sqlparse-0.4.4 tzdata-2023.3
WARNING: There was an error checking the latest version of pip.
```

## 验证安装

方法一、
```bash
(venv) PS D:\DevSpace\Python\Project\djangoweb> python -m django --version
4.2
```
方法二、

```bash
(venv) PS D:\DevSpace\Python\Project\djangoweb>python
Python 3.11.3 (tags/v3.11.3:f3909b8, Apr  4 2023, 23:49:59) [MSC v.1934 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> import django
>>> print(django.get_version())
4.2
>>>
```