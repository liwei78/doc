### nginx init script


/etc/init.d/nginx

chmod 755 nginx

chkconfig nginx on

chkconfig --list nginx


### linux os 将操作环境分为以下7个等级:

* 0:开机(请不要切换到此等级)
* 1:单人使用者模式的文字界面
* 2:多人使用者模式的文字界面,不具有网络档案系统(NFS)功能
* 3:多人使用者模式的文字界面,具有网络档案系统(NFS)功能
* 4:某些发行版的linux使用此等级进入x windows system
* 5:某些发行版的linux使用此等级进入x windows system
* 6:重新启动

Linux中有多种运行级，常见的就是多用户的2，3，4，5 ，很多人知道5是运行X-Windows的级别，而0就是关机了。运行级的改变可以通过init命令来切换。例如，假设你要维护系统进入单用户状态，那 么，可以使用init1来切换。在Linux的运行级的切换过程中，系统会自动寻找对应运行级的目录/etc/rc[0-6].d下的K和S开头的文件， 按后面的数字顺序，执行这些脚本。对这些脚本的维护，是很繁琐的一件事情，Linux提供了chkconfig命令用来更新和查询不同运行级上的系统服 务。
