Nagios

## Role Variables

The variables you can configure are listed below. For the default settings you can look in `deafult/main.yml`.


This is the directory where the downloaded files will be placed and extracted.

    nagiosurl: https://assets.nagios.com/downloads/nagioscore/releases/nagios-4.2.4.tar.gz
    nagiossrc: nagios-4.2.4

The download url for Nagios along with the directory name which will be created when the source file is
decompressed to. I.e. with `tar -xzvf nagios-4.1.1.tar.gz`

    pluginsurl: https://nagios-plugins.org/download/nagios-plugins-2.1.4.tar.gz
    pluginssrc: nagios-plugins-2.1.4

apache_service: httpd
apache_user: apache
iptables_service: iptables
with_httpd_conf: /etc/httpd/conf.d
      
The users which should be allowed to login to the Nagios web GUI.

## Dependencies

None.

## Example Playbook

Install Nagios and setup the password for your nagios admin user.

	- hosts: monitoring-servers
	  become: yes
 	  vars_files:
		- roles/nagios/vars/main.yml
	  roles:
		- iptables
		- ntp
		- nagios

*Contents of vars/main.yml*:

    nagios_users:
	- user: jainendra
	  pass: jainendra

    download_dir: /home/jainendra/nagios

    monitoring_user: jainendra
    monitoring_command_group: jainendra

