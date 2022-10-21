### Quick Start:

1. Start by cloning the repo to the machine you want to install Guacamole: 

`git clone https://github.com/ajay75/guacamole-ansible.git`

2. Run `./setup.sh`

3. That's it, you will be asked to supply a password for MySQL and the GuacD daemon.  The rest will be completed automatically.
4. To debug the RDP connection if fails to work at command line, make sure all the following services running and guacd log messages will give your insight information.


```shell
sudo grep guacd /etc/log/messages | tail -n 30 
sudo systemctl status guacd
sudo systemctl status tomcat9
sudo systemctl staus mariadb
```

### Supported Linux Distros:
- CentOS 7
- CentOS 8
- RHEL 7
- RHEL 8
- Rocky Linux 8
- Oracle Linux 7
- Oracle Linux 8
- Debian 11
- Ubuntu 20.04

