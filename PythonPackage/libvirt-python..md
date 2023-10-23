## libvirt-python
libvirt是一个开源的虚拟化API库，它允许管理不同的虚拟化技术，如KVM和QEMU。libvirt-python是libvirt库的Python绑定，提供了在Python中使用libvirt的接口

## Links
- 官方Pypi源
    -  https://pypi.org/project/libvirt-python/
- 清华大学开源镜像站Pypi源
    - https://pypi.tuna.tsinghua.edu.cn/simple/libvirt-python/

## Install
前提：系统已安装libvirt相关包，以及python-devel包。
```bash
pip install libvirt-python
```
**PS**
1. 安装libvirt相关包
```bash
# CentOS
$ sudo yum install libvirt*
```
2. 安装python-devel包
```bash
#CentOS
$ sudo yum -y install python-devel

#Ubuntu
$ sudo apt-get install python-dev

#python3使用python3-dev
```
