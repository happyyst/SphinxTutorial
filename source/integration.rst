4. 托管与集成
========

无论是markdown还是reST, 在github上都能得到不错的支持.

文档托管
----

readthedocs是一个sphinx文档托管站点. 支持从git, github, svn导入项目
以下以github为例, 讲述文档的托管

#. 注册readthedocs账号
#. 在readthedocs中新建项目

    * 新建项目
    .. image:: _static/step1.jpg

    * 手动导入
    .. image:: _static/step2.jpg

    * 填写项目名称和地址
    .. image:: _static/step3.jpg

#. github中启用webhook, 通知readthedocs自动构建

    .. image:: _static/step4.jpg