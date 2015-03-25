Odoo-openerp-install-scripts
Odoo一键安装脚本.sh
=======================

ODOO v8 install script | Github | Ubuntu 14.04 LTS
作者： André Schenkels / 距今日2015-03-25约258天前发文 /


我整了这脚本儿，可一键把odoo安到ubuntu 14 server里头去。非常好使，腰也不酸了，腿也不疼了，一气儿上6楼，DuangDuangDuang就上去了!
 

脚本sh我放在这儿了：

https://github.com/aschenkels-ictstudio/openerp-install-scripts/blob/master/odoo-v8/ubuntu-14-04/odoo_install.sh

有了脚本儿方便了，但您老还得注意点那啥，下边儿给您罗列一下用药注意事项：

版本要注意：

Odoo的版本儿挑： 8.0 或者 master (trunk)呗！

完事之后，在Odoo里的配置设定项上边，

OE_USER: 得创建一个deamon uses用户账号（废话）

OE_HOME: 得有一文件夹用来装odoo（更废话）

OE_CONFIG: Odoo的conf配置文件（这个必须得有）

如果你把一脚安装脚本粘贴到一个名叫【 odoo_install.sh 的文件里头了，那么

你得给这sh文件权限，给权限的命令如下：

chmod +x odoo_install.sh

然后运行这个脚本sh：

./odoo_install.sh

如果上述一切正常的话，那么你就可以从浏览器输入类似这个URL网址来访问odoo啦： http://ipadress-server:8069

当然了，要是您想停止odoo或者开机就启动odoo，就得参考 /etc/init.d/odoo-server stop (停止) 或者 /etc/init.d/odoo-server (启动)啦。后边的不教，教会学生，饿死老湿！
