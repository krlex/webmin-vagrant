# The Webmin in Vagrant

Webmin is a web-based system configuration tool for Unix-like systems,
although recent versions can also be installed and run on Microsoft Windows.
Webmin allows the user to configure operating system internals, such as users, 
disk quotas, services or configuration files, as well as modify and control 
open-source apps, such as the Apache HTTP Server, PHP or MySQL.

## Installation and configuration

Before you provisioning installation and configuration you need to add hostname in hosts

```
echo "192.168.33.10  ubuntu-focal" >> /etc/hosts
```
and then:

```
vagrant up
```
or if you have error without provision you need to do:

```
vagrant status
```
if is vagrant running you need to do this:

```
vagrant provision
```
and after provisioning vagrant will reboot and after few minutes you can go to:

in browser 

https://ubuntu-focal:10000

### Warning

Your username and password of webmin is a same as of user and password of you machine.
In this case is:

username: vagrant
password: vagrant
