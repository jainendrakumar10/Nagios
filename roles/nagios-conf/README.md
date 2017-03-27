Nagios Server Config
=========

Requirements
------------
	none

Role Variables
--------------
	nagios_user: jainendra
	nagios_group: jainendra


some_dict:

	host1:
		index: 0
		name: nrpe1_centos7
		nrpe_hostadd: ""
		nrpe_ip: ""

	host2:
		index: 1			#Sequential index number
		name: nrpe2_centos7						#Name to be displayed on dashboard
		nrpe_hostadd: ""		#Fully Qualified Domain Name of remote host
		nrpe_ip: ""						#IP Address of remote host


Dependencies
------------

N/A

