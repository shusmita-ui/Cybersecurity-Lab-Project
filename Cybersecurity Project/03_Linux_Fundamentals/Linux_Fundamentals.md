# Linux Fundamentals


## Objective


To understand basic Linux filesystem navigation, file permissions, package management, and networking commands.


---


## 1. File System Navigation


### pwd


The `pwd` command displays the current working directory.


```bash
pwd
ls

The ls command lists files and directories

ls
cd

The cd command is used to change the current directory.

cd /var/www/html
2. File and Directory Permissions

Linux uses permissions to control access to files and directories.

The three basic permissions are:

Read (r)
Write (w)
Execute (x)
chmod

The chmod command changes file or directory permissions.

Example:

chmod 755 filename
chown

The chown command changes the ownership of a file or directory.

Example:

sudo chown user:user filename
3. Package Management

Kali Linux uses Debian-based package management.

apt

The apt command is used to update, install, and remove packages.

Update package information:

sudo apt update

Install a package:

sudo apt install package-name
dpkg

The dpkg command is used to install and manage Debian packages.

Example:

sudo dpkg -i package.deb
4. Networking Commands
ip

The ip command is used to view network interfaces and routing information.

ip addr

To view the routing table:

ip route
ping

The ping command checks whether another host is reachable over the network.

Example:

ping 192.168.133.128
ss

The ss command displays network connections and listening ports.

Example:

ss -tuln
traceroute

The traceroute command shows the path packets take to reach a destination.

Example:

traceroute example.com
5. Practical Work

The following Linux commands were practiced in the laboratory:

pwd
ls
cd
chmod
chown
apt
dpkg
ip
ping
ss
traceroute