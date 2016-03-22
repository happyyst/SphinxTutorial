.. project documentation master file, created by
   sphinx-quickstart on Mon Mar 21 10:44:29 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.
..  toctree::
    intro
    install
    basic
    doctor
    codeblock

Welcome to project's documentation!
===================================


单星号: *文本* 得 强调 (斜体 对中文一般效果不好)

双星号: **文本** 得 加重 (加黑),

反引号: ``文本`` 得 代码引用.



.. highlight:: html

The literal blocks are now highlighted as HTML, until a new directive is found.

::
   <html><head></head>
   <body>This is a text.</body>
   </html>

The following directive changes the hightlight language to SQL.

.. highlight:: sql

::
   SELECT * FROM mytable

.. highlight:: none

From here on no highlighting will be done.

::
   SELECT * FROM mytable



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

