# Lab Environment Setup

## Objective

To create a controlled and isolated cybersecurity laboratory for practical security testing and learning.

## Virtualization Platform

VMware was used to create and manage the virtual machines.

## Attacker Machine

**Kali Linux**

Kali Linux is a security-focused Linux distribution containing tools for penetration testing, network analysis, vulnerability assessment, and digital forensics.

## Target Machine

**Metasploitable2**

Metasploitable2 is an intentionally vulnerable virtual machine used for authorized security testing and learning.

## Web Application Target

**DVWA (Damn Vulnerable Web Application)**

DVWA is an intentionally vulnerable web application used to practice web application security concepts in a controlled environment.

## Network Configuration

The lab uses a private Host-only network for communication between the attacker and target machines.

### Kali Linux

- NAT interface: `192.168.241.130`
- Host-only interface: `192.168.133.129`

### Metasploitable2

- Host-only IP: `192.168.133.128`

### Host-only Network

- Network: `192.168.133.0/24`
- Subnet Mask: `255.255.255.0`

## NAT

NAT provides Kali Linux with controlled Internet connectivity through the host system.

## Host-only Network

The Host-only network allows communication between the virtual machines while keeping the target environment isolated from the physical network.

## Connectivity Test

The connection between Kali Linux and Metasploitable2 was verified using the `ping` command.

## Result

The virtual cybersecurity lab was successfully configured and the attacker and target machines were able to communicate through the isolated network.