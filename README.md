SSH/SCP App - connect
===========

This is a shell utility. It can be used to connect servers with passwords. It leverages native sshpass. It takes "ssh" or "scp" as an argument to act accordingly.


Prerequisites
------------------
- Install these via your platform's preferred method (apt, yum, ports, emerge, etc.):

	sshd

- Connectivity to other server on port 22.

Properties
-----------
- poclabapps.properties

  -  It requires this property file to define all servers and properties.

	apps="stackstorm vcpe odl vdx icx bfo icx2 sdn email"

	root_apps="email stackstorm vcpe odl bfo sdn"

	admin_apps="vdx icx icx2"

	root_user="root"

	root_password="root"

	admin_user="admin"

	admin_password="password"

	Apps Information
	-----------------------

	stackstorm="10.88.88.140"
	
	vcpe="10.88.88.161"
	
	odl="10.88.88.141"

Usage
---------

- when connecting through ssh:
	
	connect ssh {applications}
or

- when connecting through scp:
	
	connect scp {applications} {dir_location_for_all_files}

Supports
------------

	MacOSX
	Redhat
	CentOS
	Ubuntu
	Debian

License
-----------
connect is released under the APACHE 2.0 license. See LICENSE for more information.