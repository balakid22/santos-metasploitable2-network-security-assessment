# Metasploitable 2 Network Security Assessment

## Overview

This project documents an authorized network security assessment performed against an intentionally vulnerable Metasploitable 2 virtual machine.

The assessment was conducted in an isolated VirtualBox Host-only network using Kali Linux as the analyst machine.

## Lab Architecture

```text
Kali Linux VM
IP: 192.168.182.4
        |
        | VirtualBox Host-only Network
        |
Metasploitable 2 VM
IP: 192.168.182.3
```


## Objectives
- Verify connectivity between Kali Linux and Metasploitable 2
- Identify open ports and exposed services
- Detect service and version information
- Capture and analyze TCP and HTTP traffic
- Document security observations and recommendations


## Tools Used
- Kali Linux
- Nmap
- Wireshark
- VirtualBox
- GitHub


## Methodology
1. Configured Kali Linux and Metasploitable 2 using a VirtualBox Host-only network.
2. Verified connectivity using ping.
3. Performed a basic Nmap scan.
4. Performed service and version detection.
5. Performed a detailed Nmap scan using default scripts.
6. Captured traffic using Wireshark.
7. Analyzed TCP and HTTP traffic.
8. Documented findings and recommendations.


## Scope and Authorization
All testing was conducted against an intentionally vulnerable virtual machine owned and controlled by the student.
The assessment was limited to the isolated VirtualBox Host-only lab environment.
No public websites, external IP addresses, school networks, or third-party systems were scanned.


## Main Observations
- The Metasploitable 2 target was reachable from Kali Linux.
- Multiple TCP services were exposed on the target.
- Nmap identified service names and version information.
- Wireshark captured TCP traffic between the analyst and target machines.
- HTTP traffic to the target was visible during packet analysis.
- Unnecessary services should be disabled or restricted in a real production environment.

## PROJECT STRUCTURE
```text
## Project Structure

```text
.
├── README.md
├── report/
│   └── security-assessment.md
├── scans/
│   ├── .gitkeep
│   ├── basic-scan.md
│   ├── service-detection.md
│   └── detailed-scan.md
└── screenshots/
    ├── .gitkeep
    ├── Successful-ping.png
    ├── ip-address-kali.png
    ├── ip-address-meta.png
    ├── nmap-basic-scan.png
    ├── nmap-service-detection1.png
    ├── nmap-service-detection2.png
    ├── nmap-service-detection3.png
    ├── virtualbox-network-setup-kali.png
    ├── virtualbox-network-setup-meta.png
    ├── wireshark-http-traffic.png
    ├── wireshark-tcp-analysis.png
    └── wireshark-tcp-analysis2.png
```
```

## Evidence
The repository includes:
- Nmap scan outputs
- VirtualBox network configuration screenshots
- Connectivity verification screenshots
- Wireshark TCP and HTTP traffic screenshots
- A technical security assessment report


## Limitations
- Testing was performed only against an authorized virtual machine.
- The target was intentionally vulnerable for educational purposes.
- No exploitation or brute-force testing was performed.
- The assessment does not represent a complete enterprise security assessment.


## Conclusion
This project demonstrated basic network reconnaissance, service identification, TCP traffic analysis, HTTP inspection, and technical security documentation using Kali Linux, Nmap, Wireshark, and VirtualBox.
