## Pip
pip 是 Python 的软件包安装程序。您可以使用它来 从 Python 包索引和其他索引安装包。

## Pip Links
官网文档：[https://pip.pypa.io/en/stable/](https://pip.pypa.io/en/stable/)
Pip命令：[https://pip.pypa.io/en/stable/cli/](https://pip.pypa.io/en/stable/cli/)

## Pip安装
官网安装：[https://pip.pypa.io/en/stable/installation/](https://pip.pypa.io/en/stable/installation/)
官网Linux包管理器：[https://packaging.python.org/en/latest/guides/installing-using-linux-tools/](https://packaging.python.org/en/latest/guides/installing-using-linux-tools/) 

- **get-pip.py**
    ```bash
    $ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
    $ python3 get-pip.py --user
    ```

- **Linux包管理器**
   - Debian/Ubuntu
    ```bash
    $ sudo apt update
    $ sudo apt install python3-venv python3-pip
    ```
## Pip升级

- **Linux**
    ```bash
    $ python -m pip install --upgrade pip
    ```
## Pip版本
    ```bash
    $ python3 -m pip -V
    ```
## Pip换源
常用pip镜像源：

- 阿里云 http://mirrors.aliyun.com/pypi/simple/ 
- 中国科技大学 https://pypi.mirrors.ustc.edu.cn/simple/ 
- 豆瓣(douban) http://pypi.douban.com/simple/ 
- 清华大学 https://pypi.tuna.tsinghua.edu.cn/simple/ 
- 中国科学技术大学 http://pypi.mirrors.ustc.edu.cn/simple/
```bash
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple/ 
```
```bash
#pip换源
$ cd ~             
$ mkdir .pip      
$ vim .pip/pip.conf
# pip 清华源
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
[install]
trusted-host = https://pypi.tuna.tsinghua.edu.cn
```

## Pip使用

安装与卸载库
```bash
$ pip install xxxx
$ pip uninstall xxxx
```