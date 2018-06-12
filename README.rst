Selenium2Library
================

Selenium2Library 库是`Robot Framework`的Web测试库
在内部使用Selenium_ tool。该项目由GitHub下载.也可以从PyPI_找到。

从3.0版本开始，将Selenium2Library改名为SeleniumLibrary
这个项目主要用于帮助过渡。

版本
--------

Selenium2Library 3.0 和更新SeleniumLibrary包含完全相同的代码和功能。已经有很多
library内部的变化，但外部的功能关键词应该完全向后兼容。library和tools使用内部的Selenium2Library可能需要更新以支持.然而，Selenium2Library 3.0, though. Selenium2Library 1.8是最新的，也是最后一个，旧版本与旧的架构和代码。

Selenium2Library 3.0支持Python 2.7以及Python 3.3和更新。
Selenium2Library 1.8支持Python 2.62.7。

关键词文档
--------------------

- `Selenium2Library 3.0`__ (latest)
- `Selenium2Library 1.8`__ (legacy)

__ http://robotframework.org/Selenium2Library/Selenium2Library.html
__ http://robotframework.org/Selenium2Library/Selenium2Library-1.8.0.html

安装
--------------

不管版本如何，推荐安装Selenium2Library的方法，
正在使用PIPI。

安装（或升级）最新的Selenium2Library版本：

	pip install --upgrade robotframework-selenium2library

安装传统的Selenium2Library 1.8.0 版本：

	pip install robotframework-selenium2library==1.8.0

迁移到SeleniumLibrary
------------------------

现有的Selenium2Library用户应该开始迁移到
SeleniumLibrary对于大多数用户来说，这应该是一个简单的过程：

1。安装上面所解释的最新的Selenium2Library。此安装
SeleniumLibrary和Selenium2Library，事实上Selenium2Library
现在对SeleniumLibrary来说只是一个薄薄的包装纸。

2。通常执行测试以查看是否存在问题。

三。如果遇到问题，试着调查它们为什么会发生。可能的
问题可分为两类：

-如果库本身提供的关键字已经更改，请查看
“SeleniumLibrary3.0版本注释”参见
不相容的变化。如果不是，你可能遇到了回归。
这应该被报告为“SeleniumLibrary问题跟踪器”。

如果Selenium2Library无法使用，很有可能是由于selenium2library3.0内部变化很大，报告给seleniumlibrary维护人员的问题以解决问题。如果你是维护者。你可以在各种“支持”上寻求帮助。

4。如果没有问题发生或问题解决后，你就可以开始了。
更改库导入使用“SeleniumLibrary”代替
‘Selenium2Library’。同样的所有关键字使用形式
‘Selenium2Library的标题应该是‘需要更新’。

5。在测试数据被更新后，Selenium2Library可以删除。

.. _Robot Framework: http://robotframework.org
.. _Selenium: http://seleniumhq.org
.. _PyPI: https://pypi.python.org/pypi/robotframework-selenium2library
.. _GitHub: https://github.com/robotframework/Selenium2Library
.. _SeleniumLibrary: https://github.com/robotframework/SeleniumLibrary
.. _pip: http://pip-installer.org
.. _SeleniumLibrary 3.0 release notes: https://github.com/robotframework/SeleniumLibrary/blob/master/docs/SeleniumLibrary-3.0.0.rst
.. _SeleniumLibrary issue tracker: https://github.com/robotframework/SeleniumLibrary/issues
.. _support channels: http://robotframework.org/#support
