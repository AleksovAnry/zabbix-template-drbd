DRBD Resources monitoring template for Zabbix
=============================================

Using _drbdadm_ tool for monitoring of DRBD Resources

Tested on Zabbix Version 6.0
Tested on DRBD 8.4.x

FEATURES
--------
* LLD for DRBD Resources
* Monitoring of Role, Device state and Connection state
* Triggers for degraded situation

REQUIREMENTS
------------
* Zabbix server version 3.0
* drbdadm tool

INSTALLATION
------------
* Agent on DRBD server
  * Copy __userparameter_drbd.conf__ to __/etc/zabbix/zabbix_agentd.d/userparameter_drbd.conf__
  * Modify /etc/sudoers file to include directives from __sudo__ file (or fill in __/etc/sudoers.d/zabbix__ if supported. Remember to chmod it to 0440 for safety reasons)
  * Restart zabbix agent
* Zabbix server
  * Import template __zbx_drbd_templates.yaml__ file

AUTHOR
------
Original author: Stefano Buelow - stefano.buelow@gmail.com
Adopt author: Aleksov Anry - aleksov@set-pro.net

LICENSE
-------
GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007

See [LICENSE](LICENSE)

