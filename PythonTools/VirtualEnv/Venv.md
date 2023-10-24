## Venv
venv该模块支持创建轻量级的“虚拟环境”， 每个都安装了自己独立的一组 Python 包 他们的目录。 在现有环境之上创建虚拟环境 Python安装，被称为虚拟环境的“基础”Python，并可能 （可选）与基本环境中的包隔离， 因此，只有那些明确安装在虚拟环境中的那些才可用。

## Links

- PythonWiki：[https://docs.python.org/3/library/venv.html](https://docs.python.org/3/library/venv.html)
- Blog：
   - [python多环境管理（venv与virtualenv） - doublexi - 博客园](https://www.cnblogs.com/doublexi/p/15783355.html)
   - [Python 虚拟环境: 如何创建、激活、停用和删除？ | 嘻嘻IT](https://www.11meigui.com/2023/python-venv.html)
   - [venv](https://www.liaoxuefeng.com/wiki/1016959663602400/1019273143120480)

---

## 安装
自 3.3 版本之后添加的官方库，自 3.6 版本之后，成为官方推荐的多环境管理工具。也就是说，你不需要安装任何第三方库就可以实现多环境管理了。**注意：python3.3版本之后自带的模块，只支持3.3版本之后的，不支持2.x**
## 使用

- **创建venv环境**

```bash
$ python3 -m venv . #在当前目录创建venv环境
$ python3 -m venv venvname #创建一个名为venvname的venv环境

$ ls venvname
bin  include  lib  lib64  pyvenv.cfg  share

#venv的软件包管理目录site-package在lib/python3.6/site-packages/下。
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
