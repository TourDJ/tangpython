
### python 常用命令
查看使用pip安装的软件包:

    pip list
    pip freeze

查看指定版本的pip安装的软件包:

    python2 -m pip list
    python3 -m pip list

查看pip安装的软件包路径:

    pip show xkit

将pip freeze的内容输出至requirements.txt

    pip freeze | tee requirements.txt # 输出本地包环境至文件
    pip install -r requirements.txt # 根据文件进行包安装
