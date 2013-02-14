named
=====

Use this repo to create a basic dns server

On an EC2, make sure that named.conf is placed in /etc/

While the rest of the files/ directories should go into /var/named/ 

I used this for creating a DNS Server in a VPC. It proxies the request it cannot resolve. 

VPC Subnet used for testing is 172.16.7.0/24. Make sure you are using the same subnet. If not change the subnet in 

	- named.conf
	- zone.net.yourdomainname

AND

	- Create a file to replace, revp.172.16.7 in /var/named/ 
