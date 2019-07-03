x-studio365 - CSD恢复
=====================

.. important:: ``导入时选择目录`` + ``csb引用图片相对路径`` = ``图片在磁盘的绝对路径``；**只有符合这条规则，导入后，软件才可以正常加载到图片。**


1. 通过软件主菜单【文件】【新建工程】新建一个空UI工程，如图所示：

   |figure_1|

#. 通过软件主菜单【文件】【导入】【CocosStudio(*.csb/*.json)】导入资源目录

   资源根目录确定方法: 在系统资源管理器右键【Open with x-studio365】打开待导入资源随便一个.csb
   如图所示：

   |figure_2|

   打开后显示如图所示：

   |figure_3|
   虽然是乱码，但我们依然可以看到csb引用到的图片的相对路径。如上图所示，我们可以确定导入时应该选择
   ``D:\dev\tmp\res-20190304\res`` 。

#. 查看导入界面，调整设计尺寸

   导入完成后，记得在 **资源视图** 双击打开界面，如果界面显示不全请修改和原界面相同尺寸，
   原界面设计尺寸可在对象探查器查看根节点属性大小来确定, 如图所示:

   |figure_4|

#. 发布.ccs工程
   通过软件主菜单【工程】【发布】发布到CocosStudio2.x兼容的.ccs工程，
   **注意: 发布选项里CSLoader版本一定要选择2.1.0.0**，
   如果不确定，可以通过软件主菜单【工程】【工程设置】打开发布选项对话框，如图所示：

   |figure_5|

#. 使用CocosStudio2.3.3或者3.10打开发布后的工程，如下图所示：

   |figure_6|

.. note:: 目前只支持导入CocosStudio2.x发布的.csb/json, .json/.csb均可以已纯文本方式打开查看版本信息。

.. |figure_1| image:: ../img/c3s2_01.png
.. |figure_2| image:: ../img/c3s2_02a.png
.. |figure_3| image:: ../img/c3s2_02b.png
.. |figure_4| image:: ../img/c3s2_03.png
.. |figure_5| image:: ../img/c3s2_04.png
.. |figure_6| image:: ../img/c3s2_05.png
