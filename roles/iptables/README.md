Iptables
=========

Installs a simple iptables-classic firewall for RHEL/CentOS systems.  
For EL it uses traditional iptables package and iptables service for those who doesn't like firewalld.  
  

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see vars/RedHat_7.yml):

	iptables_pkgs:
		- iptables-services
		- iptables-utils
	iptables_service: iptables
	iptables_config: '/etc/sysconfig/iptables'


Dependencies
------------
	None.

License
-------
	None

Author Information
------------------
	compose team
