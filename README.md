cisco_snarf
===========

Python script to make it easy to backup configurations on a number of Cisco routers and firewalls

This utility will connect with a list of Cisco devices using the supplied
credentials and extract the configuration and some running information from
the device. It will attempt to use the protocols SSH, HTTPS, telnet and HTTP
until it gets a successful connection

Usage
=====
    Usage: cisco_snarf {options} hosts
    Options:
	-u|--username username 
	-p|--password password
	-e|--enable enable_password
	-f|--file hosts_file - Read hostnames from a file
	-m|--mechanism - Connection mechanism. Can be specified more than one. Either ssh, https, telnet or http
	-P|--prefix - File or directory prefix to use in constructing the output file names
	-d : Turn on debugging

Requires
========
- python version 2.6
- pexpect
- ssh client
