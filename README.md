# Task01
自行完成配置，在安装过程中发现黑屏无响应，经过检查发现是只有集成显卡，导致nvdia驱动错误，最后通过禁用n卡驱动完成安装。

在grub界面选择ubuntu后按e进入启动项编辑页面，后在quiet slash后添加nomodeset，F10保存并加载，即可进入图形化界面。

之后terminal内输入sudo gedit /boot/grub/grub.cfg，在quiet slash后添加nomodeset，并保存。

接下来命令行键入 sudo update-grub 即可。

完成后图片如下：
![finish](finish.png)