# MAC-Address-changer
This is a MAC Address changer python code







Subprocess Module - 

	1. The subprocess module  contains a number of functions
	2. These Functions allow us to execute system commands
	3. Commands depend of the OS which executes the scripts.

Syntax:

import subprocess
subprocess.call("COMMAND",Shell=True)


#!/usr/bin/env python

import subprocess

subprocess.call("ifconfig", shell=True)




#!/usr/bin/env python

import subprocess

subprocess.call("ifconfig eth0 down", shell=True)
subprocess.call("ifconfig eth0 hw ether 00:11:22:33:44:55", shell=True)
subprocess.call("ifconfig eth0 up", shell=True)


MAC_CHANGER Variables

	• A variable is a location in memory that contains a certain value
	• Similar to maths, it’s a name that is used to store information.


#!/usr/bin/env python

import subprocess

Interface = "eth0"
New_MAC = "00:11:22:33:44:66"

Print("[+] Changing MAC address for " + Interface + " to " + New_MAC)

#subprocess.call("ifconfig eth0 down", shell=True)
#subprocess.call("ifconfig eth0 hw ether 00:11:22:33:44:55", shell=True)
#subprocess.call("ifconfig eth0 up", shell=True)





#!/usr/bin/env python

import subprocess

Interface = "eth0"
New_MAC = "00:11:22:33:44:66"

Print("[+] Changing MAC address for " + Interface + " to " + New_MAC)

subprocess.call("ifconfig " + interface + " down", shell=True)
subprocess.call("ifconfig " + interface + " hw ether " + New_MAC, shell=True)
subprocess.call("ifconfig " + interface + " up", shell=True)
![image](https://github.com/user-attachments/assets/11029131-7fd3-4526-b9e5-78f57aabc9c8)
