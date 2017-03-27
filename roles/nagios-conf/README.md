Nagios Server Config
=========

Requirements
------------
	none

Role Variables
--------------
	nagios_user: compose
	nagios_group: compose


some_dict:

	host1:
		index: 0
		name: nrpe1_centos7
		nrpe_hostadd: "ip-172-31-9-14.us-west-2.compute.internal"
		nrpe_ip: "172.31.9.14"

	host2:
		index: 1			#Sequential index number
		name: nrpe2_centos7						#Name to be displayed on dashboard
		nrpe_hostadd: "ip-172-31-4-146.us-west-2.compute.internal"		#Fully Qualified Domain Name of remote host
		nrpe_ip: "172.31.4.146"						#IP Address of remote host


Dependencies
------------

N/A

