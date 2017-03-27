Nagios and nrpe
=========

Requirements
------------

	centos7

	Add below line into /etc/sudoers on target machine after "Same thing without a password"

	compose ALL=(ALL) NOPASSWD: ALL

	add host ip into /etc/hosts file

	add nagios and nrpe serever ip into inventory/nagios-servers


Role Variables
--------------

Dependencies
------------
	epel-release

	iptables

	ntp

How to run Playbook
----------------
		[compose@centos66 ansible-compose-nagios]$ ansible-playbook  site.yml -i inventory/nagios-servers
 
License
-------

None

Author Information
------------------
compose

