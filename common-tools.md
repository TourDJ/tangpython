
## virtualenvwrapper

virtualenv 用于创建独立的Python环境，多个Python相互独立，互不影响；Virtaulenvwrapper 是virtualenv的扩展包，用于更方便管理虚拟环境。

### virtualenvwrapper install

    $ pip install virtualenvwrapper
    ...
    $ export WORKON_HOME=~/Envs
    $ mkdir -p $WORKON_HOME
    $ source /usr/local/bin/virtualenvwrapper.sh
    $ source ~/.local/bin/virtualenvwrapper.sh (for ubuntu18+)
    $ source /usr/bin/virtualenvwrapper.sh (for CentOS7)

## 创建虚拟环境

    mkvirtualenv env1
    mkvirtualenv --python=python3.5 venvname    # --python指定Python解释器程序路径

## list available environments

    workon
    workon env1

## 激活和解除

    source env1/bin/activate
    deactivate

## 删除虚拟环境

    rmvirtualenv env1

## 在虚拟环境中安装软件
Now we can install some software into the environment.

    (env1)$ pip install django
    Downloading/unpacking django
      Downloading Django-1.1.1.tar.gz (5.6Mb): 5.6Mb downloaded
      Running setup.py egg_info for package django
    Installing collected packages: django
      Running setup.py install for django
        changing mode of build/scripts-2.6/django-admin.py from 644 to 755
        changing mode of /Users/dhellmann/Envs/env1/bin/django-admin.py to 755
    Successfully installed django

We can see the new package with lssitepackages:

    (env1)$ lssitepackages
    Django-1.1.1-py2.6.egg-info     easy-install.pth
    setuptools-0.6.10-py2.6.egg     pip-0.6.3-py2.6.egg
    django                          setuptools.pth


