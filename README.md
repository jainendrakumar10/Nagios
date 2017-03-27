Nagios and nrpe
=========

Requirements
------------

	centos7

	Add below line into /etc/sudoers on target machine after "Same thing without a password"

	jainendra ALL=(ALL) NOPASSWD: ALL

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
		[jainendra@centos66 Nagios]$ ansible-playbook  site.yml -i inventory/nagios-servers
 
License
-------

NA

Author Information
------------------
NA

