# Security Tool Familiarization

## Objective

To understand the purpose and basic usage of common cybersecurity, network analysis, and web security tools.

---

## 1. Nmap

Nmap (Network Mapper) is a network scanning and enumeration tool.

### Main Uses

- Host discovery
- Port scanning
- Service detection
- Network enumeration

### Basic Command

```bash
nmap <target-ip>

Practical Work

Nmap was used to scan the intentionally vulnerable Metasploitable2 target in the isolated laboratory network.

2. Wireshark

Wireshark is a network protocol analyzer used to capture and inspect network packets.

Main Uses
Packet capture
Protocol analysis
Network troubleshooting
Traffic inspection
Practical Work

Wireshark was used to capture and analyze network traffic in the laboratory.

The following traffic was observed:

ICMP packets
HTTP packets

This helped demonstrate how network communication appears at packet level.

3. Burp Suite

Burp Suite is a web application security testing platform.

Main Uses
Intercept HTTP requests
Inspect HTTP responses
Analyze web traffic
Test web applications
Modify requests in an authorized testing environment
Practical Work

Burp Suite was configured as a web proxy and used to observe HTTP requests generated while interacting with DVWA.

The HTTP history feature was used to inspect captured requests.

4. Netcat

Netcat is a command-line networking utility used for TCP/UDP communication and basic network troubleshooting.

Main Uses
Test network connectivity
Create TCP/UDP listeners
Send and receive data
Troubleshoot network services
Listener Example
nc -lvnp 4444
Client Example
nc <target-ip> 4444
Practical Work

A basic Netcat listener and client test was performed in the laboratory to verify TCP connectivity.

5. DVWA

DVWA stands for Damn Vulnerable Web Application.

It is an intentionally vulnerable web application designed for security education and authorized penetration-testing practice.

Practical Work

DVWA was installed and accessed locally through the Apache web server.

The security level was configured to Low for basic web security exercises.

6. Tool Summary
Tool	Main Purpose
Nmap	Network and port scanning
Wireshark	Packet capture and analysis
Burp Suite	Web proxy and HTTP analysis
Netcat	Network connectivity and debugging
DVWA	Web application security practice
7. Laboratory Result

The following security tools were successfully practiced:

Nmap
Wireshark
Burp Suite
Netcat
DVWA

These tools provided practical experience in network scanning, packet analysis, web traffic inspection, network troubleshooting, and web application security testing.

Conclusion

Basic security-tool familiarization was successfully completed in the controlled cybersecurity laboratory. All activities were performed against the authorized virtual machines and intentionally vulnerable applications used for this project.