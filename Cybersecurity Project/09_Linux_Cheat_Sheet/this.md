# Linux Networking & Security Cheat Sheet

## 1. File System Navigation

| Command | Purpose | Example |
|---|---|---|
| `pwd` | Shows current directory | `pwd` |
| `ls` | Lists files and directories | `ls` |
| `ls -la` | Lists all files with details | `ls -la` |
| `cd` | Changes directory | `cd /var/www/html` |
| `cd ..` | Moves to parent directory | `cd ..` |
| `mkdir` | Creates a directory | `mkdir test` |
| `touch` | Creates an empty file | `touch file.txt` |
| `cp` | Copies files/directories | `cp file.txt backup.txt` |
| `mv` | Moves or renames files | `mv old.txt new.txt` |
| `rm` | Removes a file | `rm file.txt` |

---

## 2. File Permissions

### chmod

Changes file or directory permissions.

```bash
chmod 755 filename

chown

Changes file ownership.

sudo chown user:user filename
Permission Types
r = Read
w = Write
x = Execute

3. Package Management
Update Packages
sudo apt update
Upgrade Packages
sudo apt upgrade
Install a Package
sudo apt install package-name
Remove a Package
sudo apt remove package-name
dpkg

Install a .deb package:

sudo dpkg -i package.deb

4. Network Information
Show IP Address
ip addr
Show Routing Table
ip route
Show Listening Ports
ss -tuln
Test Connectivity
ping <target-ip>

Example:

ping 192.168.133.128
Trace Network Path
traceroute example.com

5. DNS Commands
nslookup
nslookup example.com
dig
dig example.com
Check DNS Records
dig example.com

6. Network Scanning
Nmap Basic Scan
nmap <target-ip>
Service Detection
nmap -sV <target-ip>
Ping Scan
nmap -sn <network>

Use scanning commands only against systems you are authorized to test.

7. Network Troubleshooting
Check Interfaces
ip link
Check Routes
ip route
Test Local Connectivity
ping 127.0.0.1
Check Open/Listening Ports
ss -tuln

8. Netcat
Start TCP Listener
nc -lvnp 4444
Connect to a Listener
nc <target-ip> 4444

Netcat can be used for basic network connectivity testing and troubleshooting.

9. Process Management
Show Running Processes
ps aux
Interactive Process Monitor
top
Find a Process
ps aux | grep process-name
Stop a Process
kill <PID>

10. Service Management
Start a Service
sudo systemctl start service-name
Stop a Service
sudo systemctl stop service-name
Check Service Status
sudo systemctl status service-name
Enable Service at Boot
sudo systemctl enable service-name

11. Useful Security Commands
Check Current User
whoami
Show User ID and Groups
id
Show Logged-in Users
who
Show System Information
uname -a
Check Disk Usage
df -h
Check Memory Usage
free -h

12. File Searching
Find a File
find /path -name "filename"
Search Text in Files
grep "text" filename
Recursive Search
grep -r "text" /path
13. Hashing
MD5
md5sum file.txt
SHA-256
sha256sum file.txt

Hashing can be used to verify file integrity.

14. OpenSSL
Check Version
openssl version
Generate RSA Private Key
openssl genrsa -out server.key 2048
Generate Self-Signed Certificate
openssl req -new -x509 -key server.key -out server.crt

15. Quick Reference
pwd              → Current directory
ls               → List files
cd               → Change directory
chmod            → Change permissions
chown            → Change ownership
apt              → Package management
ip addr          → IP information
ip route         → Routing table
ping             → Connectivity test
ss -tuln         → Listening ports
traceroute       → Network path
nslookup         → DNS lookup
dig              → DNS query
nmap             → Network scanning
nc               → Network connectivity
ps aux           → Running processes
systemctl        → Manage services
whoami           → Current user
df -h            → Disk usage
free -h          → Memory usage
md5sum           → MD5 hash
sha256sum        → SHA-256 hash
openssl          → Cryptographic operations
Lab Context

These commands were practiced and used as part of a controlled cybersecurity laboratory using Kali Linux, Metasploitable2, and DVWA.

All security testing was performed only in the authorized laboratory environment.