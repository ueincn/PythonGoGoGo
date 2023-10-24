# VirtualEnv
virtualenv 是目前最流行的 python 虚拟环境配置工具。它不仅同时支持 python2 和 python3，而且可以为每个虚拟环境指定 python 解释器，并可以选择继承基础版本的包。
virtualenv 可以说是 venv 的增强版本，不过早在 venv 出现之前，virtualenv 就算是最受欢迎的命令行环境管理工具了。venv 的许多特性也是借鉴的 virtualenv，相比于 venv，其强大之处主要在：

- 更快
- 扩展性更强
- 自动发现并可创建多版本的 Python 环境
- 可通过 pip 更新
- 丰富的编程接口
## Links

- 官网：[https://virtualenv.pypa.io/en/latest/](https://virtualenv.pypa.io/en/latest/)

---

## 安装

```bash
$ pip3 install virtualenv
```
## 使用

- **创建venv环境**

```bash
$ virtualenv venvname #创建一个名为venvname的venv环境

$ ls venvname
bin  lib  pyvenv.cfg

#virtualenv的软件包管理目录site-package在lib/python3.x/site-packages/下。
```

- **激活venv环境**

| Platform | Shell | Command to activate virtual environment |
| --- | --- | --- |
| POSIX | bash/zsh | $ source _<venv>_/bin/activate |
|  | fish | $ source _<venv>_/bin/activate.fish |
|  | csh/tcsh | $ source _<venv>_/bin/activate.csh |
|  | PowerShell | $ _<venv>_/bin/Activate.ps1 |
| Windows | cmd.exe | C:\\> _<venv>_\\Scripts\\activate.bat |
|  | PowerShell | PS C:\\> _<venv>_\\Scripts\\Activate.ps1 |

- **退出venv环境**

```bash
(venv) ~$ deactivate
```

- **删除venv环境**

```bash
$ rm -rf venvname
```

- **指定python版本**

创建的虚拟环境的python解释器，默认使用virtualenv里的版本。
```bash
$ virtualenv venvname -p python3.9
```

- **继承基础环境的包**
```bash
#先在父环境，pip安装一个包jieba
$ pip3 install jieba

#创建一个可以访问基础环境包的虚拟环境
$ virtualenv --system-site-packages venvname
```
