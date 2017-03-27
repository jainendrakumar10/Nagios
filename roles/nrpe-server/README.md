Nagios NRPE Server Config
=========

Requirements
------------
	none

Role Variables
--------------

	nagios_nrpe_server_user*: nrpe
	nagios_nrpe_server_group*: nrpe

	nagios_nrpe_server_bind_address*: 127.0.0.1
	nagios_nrpe_server_port*: 5666
	nagios_nrpe_server_allowed_hosts*: 127.0.0.1


`defaults/main.yml` 

	nagios_nrpe_server_plugins_dir*: /usr/lib64/nagios/plugins
	nagios_nrpe_server_pid*: /var/run/nrpe/nrpe.pid
	nagios_nrpe_server_repo_redhat*: epel
	nagios_nrpe_server_service*: nrpe
	nagios_nrpe_server_dir*: /etc/nagios



Dependencies
------------

N/A
