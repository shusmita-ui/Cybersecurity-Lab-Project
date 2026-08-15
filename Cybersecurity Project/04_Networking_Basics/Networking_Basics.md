# Networking Basics


## Objective


To understand fundamental networking concepts including the OSI model, TCP/IP protocol suite, DNS, HTTP/HTTPS, IP addressing, subnetting, and NAT.


---


## 1. OSI Model


The OSI (Open Systems Interconnection) model explains network communication using seven layers.


| Layer | Name | Main Function |
|---|---|---|
| 7 | Application | Provides network services to applications |
| 6 | Presentation | Data formatting, encryption, and encoding |
| 5 | Session | Establishes and manages communication sessions |
| 4 | Transport | Provides end-to-end communication |
| 3 | Network | Provides IP addressing and routing |
| 2 | Data Link | Provides communication within a local network |
| 1 | Physical | Transmits raw bits over the physical medium |


---


## 2. TCP/IP Protocol Suite


The TCP/IP model is commonly divided into four layers:


1. Application
2. Transport
3. Internet
4. Network Access


### Common Protocols


- HTTP
- HTTPS
- DNS
- TCP
- UDP
- IP
- ICMP
- ARP


---


## 3. TCP and UDP


### TCP


TCP (Transmission Control Protocol) is connection-oriented and provides reliable delivery of data.


**Features:**


- Reliable communication
- Connection-oriented
- Error checking
- Ordered delivery


**Examples:**


- HTTP/HTTPS
- SSH
- FTP


### UDP


UDP (User Datagram Protocol) is connectionless and does not guarantee delivery.


**Features:**


- Faster communication
- Connectionless
- Lower overhead
- No guaranteed delivery


**Examples:**


- DNS
- DHCP
- Streaming


---


## 4. DNS


DNS stands for Domain Name System.


It converts human-readable domain names into IP addresses.


Example:


```text
example.com → IP address
Common DNS Commands
nslookup example.com
dig example.com

DNS resolution was tested during the laboratory exercises.

5. HTTP and HTTPS
HTTP

HTTP (Hypertext Transfer Protocol) is used for communication between web clients and web servers.

Default port:

80

HTTP does not provide encryption by itself.

HTTPS

HTTPS (HTTP Secure) is HTTP protected using TLS encryption.

Default port:

443

HTTPS provides:

Encryption
Authentication
Data integrity

HTTP communication with the DVWA web application was tested during the lab.

6. IP Addressing

An IP address identifies a device on a network.

Example:

192.168.133.128

The laboratory used the following private network:

Network: 192.168.133.0/24
Subnet Mask: 255.255.255.0
Host Range
192.168.133.1 – 192.168.133.254
Broadcast Address
192.168.133.255
Lab IP Addresses

Kali Linux:

192.168.133.129

Metasploitable2:

192.168.133.128
7. Subnetting

Subnetting divides a larger network into smaller logical networks.

For the laboratory:

192.168.133.0/24

The /24 prefix means that 24 bits are used for the network portion and 8 bits are available for hosts.

Subnet mask:

255.255.255.0
8. NAT

NAT stands for Network Address Translation.

NAT translates private IP addresses into addresses that can communicate with an external network.

In this laboratory, the Kali Linux NAT interface was used to provide controlled Internet connectivity.

9. Host-only Network

A Host-only network creates an isolated virtual network between the host machine and virtual machines.

In this laboratory, the Host-only network was used for communication between:

Kali Linux
Metasploitable2

This helps prevent the intentionally vulnerable target from being directly exposed to the physical network.

10. Practical Work

The following networking activities were performed:

Checked IP addresses
Tested connectivity using ping
Examined routing information
Tested DNS resolution
Tested HTTP communication
Examined NAT configuration
Configured and tested a Host-only network