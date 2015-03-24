openerp-install-scripts
=======================

ODOO v8 install script | Github | Ubuntu 14.04 LTS
by André Schenkels / 258 days ago /
Share This
Facebook 0 Tweet

I created a install script for ODOO on a brand new Ubuntu 14.04 server. This script can be used for installing 8.0 and master branches

I created a install script for ODOO on a brand new Ubuntu 14.04 server. This script can be used for installing 8.0 and master branches of the ODOO server.

The install script can be found here:

https://github.com/aschenkels-ictstudio/openerp-install-scripts/blob/master/odoo-v8/ubuntu-14-04/odoo_install.sh

In the script there are some parameters you can set at this time:

Versions

OE_VERSION: choose the ODOO version you want to install 8.0 or master (trunk)

General OpenERP Settings

OE_USER: the user the odoo deamon uses

OE_HOME: the folder where the odoo-server resides

OE_CONFIG: the name of the config file

If you want to use the script copy the file to the server or paste the contents in a odoo_install.sh file.

Make the file executable

chmod +x odoo_install.sh

and start with

./odoo_install.sh

If you have run the script you should have a working ODOO server wich is available at: http://ipadress-server:8069

The server will auto start on reboot and you can start en stop the OpenERP server with /etc/init.d/odoo-server stop (to stop) or /etc/init.d/odoo-server (to start)
