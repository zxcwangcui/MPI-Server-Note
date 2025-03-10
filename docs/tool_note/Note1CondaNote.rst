.. CondaNote

.. image:: https://visitor-badge.glitch.me/badge?page_id=lu.readthedocs.io.ServerNote.CondaNote

.. image:: https://docs.conda.io/en/latest/_images/conda_logo.svg

Package, dependency and environment management for any language—Python, R, Ruby, Lua, Scala, Java, JavaScript, C/ C++, FORTRAN, and more.


Conda 笔记
=============

Conda是一个软件包和环境管理系统，易用，开源，跨平台。

我主要使用 Conda 来管理 Python 环境，配置 CUDA 。

当然，pip + 手装 CUDA 也可以但麻烦。

    更多细节请阅读官方文档：https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/index.html

基础命令
-----------

安装、升级、卸载

.. code-block:: bash

    conda install 张三

    conda update 张三

    conda remove 张三

环境管理
------------

新建、激活、列表、移除

.. code-block:: bash

    conda create -n 名字

    conda activate 名字

    conda env list

    conda env remove -n 名字

加点细节
------------

安装 install

.. code-block:: bash

    conda install 张三

    conda install 张三=版本

    conda install 张三 李四=2.0 王五

    conda install 张三 -c 指定频道
    conda install 张三 -c conda-forge

升级 update

.. code-block:: bash

    conda update 张三
    conda update 张三=版本

    # 升级所有包
    conda update --all

卸载 remove

.. code-block:: bash

    conda remove 张三

    conda remove 张*

搜索 search

.. code-block:: bash

    conda search 某某某

    # 如
    conda search scikit-learn
    conda search pillow

列出包

.. code-block:: bash

    # 所有已安装的
    conda list

    # 列出带有 某某 的包
    conda list 某某
