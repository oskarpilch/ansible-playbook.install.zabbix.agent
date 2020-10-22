# ansible-playbook.zabbix-agent
ansible-playbook. Add and configure zabbix-agent.

Zabbix-agent 5.0 for CentOS 7, CentOS 8, RHEL 7, CentOS 8, Ubuntu 16.04 (xenial), Ubuntu 18.04 (bionic), Ubuntu 20.04 (focal)

Only for fresh installation!

You have to modify:
* zabbix-agent.yml --- hosts
* zabbix-agent2.yml --- hosts
* inventory/group_vars/zabbix.agent/main.yml --- zbx_srv

Run: ansible-playbook zabbix-agent.yml --ask-sudo-pass
Version 0.08
 - version of zabbix-agent changed to 5.0
 - added RHEL and Ubuntu 20.04
 - added zabbix-agent2 installation

Version 0.07
 - version of zabbix-agent changed to 4.4

Version 0.06
 - version of zabbix-agent changed to 4.0
 - added Debian stretch, buster; Ubuntu xenial, bionic beaver

Version 0.05
 - changed installtion zabbix-agent version from 3.2 to 3.4
 - Zabbix Vulners plugin installation
 - yml file was rename to zabbix-agent.yml

Version 0.04
 - added zabbix-agent installation
 - modified zabbix user
 - modified zabbix_agentd.conf
 - create scripts dir
 - main script moved to roles/zabbix.agent/tasks/main.yml

Version 0.03
 - added disrtibution version

Version 0.02
 - added ping hosts
 - added debug message with OS
