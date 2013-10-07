ssher
=====

SSHer is a program designed to provide the posibility of launching ssh connections from the terminal. The main objetive is to present the availables connections in an easy manner to be read. 

Install:

$ tar xvzf SSHer-1.0.tar.gz
$ cd SSHer-1.0
$ sudo python setup.py install

This will create an executable called ssher.

Once the program is installed, you have to create a configuration file. Put this configuration in:

$ vim /home/user/.ssher.cfg

[host]
username=
hostname=
ip=
tunnel=
port= 

Example of configuration:

[server01]
username=user
hostname=server01
ip=10.0.0.1
tunnel=8080:127.0.0.1:8080
port=2222


Execute:

$ ssher

| ID | HOSTNAME | IP       | USERNAME | TUNNEL | PORT |
| 1  | server01 | 10.0.0.1 | user     | 8080:127.0.0.1:8080 | 
