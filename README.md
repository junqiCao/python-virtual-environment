# python-virtual-environment
### 首先安装两个安装包

#### python 虚拟环境
`pip3 install virtualenv`
#### 封装了虚拟环境，支持一些简化命令
`pip3 install virtualenvwrapper`
#### 打开bashrc文件
`vim ~/.bashrc`
#### 在末尾添上下面的语句
```
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
export WORKON_HOME=$HOME/.virtualenvs
source ~/.local/bin/virtualenvwrapper.sh
```
#### 刷新bashrc
`source ~/.bashrc`

#### 测试
```
workon
mkvirtualenv
```
#### 注意不同点

#### 以前的配置路径(ubuntu16.04)
```source /usr/local/bin/virtualenvwrapper.sh  ```
 
#### ubuntu18.04中的配置路径
```source ~/.local/bin/virtualwrapper.sh```


和之前的pip安装的虚拟环境不同，这次是在创建python2环境时，需要指明解释器版本

#### python2环境的虚拟环境

```mkvirtualenv venv -p python2.7 venv是虚拟环境名字```

#### python3环境的虚拟环境

```mkvirtualenv venv3 venv3虚拟环境名```
```
创建虚拟环境：                mkvirtualenv 虚拟环境名称
创建虚拟环境(指定python版本)： mkvirtualenv -p python 虚拟环境名称
查看所有虚拟环境：            workon+2次tab键
使用虚拟环境：               workon 虚拟环境名称
退出虚拟环境：               deactivate
删除虚拟环境（必须先退出虚拟环境内部才能删除当前虚拟环境）: rmvirtualenv 虚拟环境名称
```
