# Metasploitable 2 Security Assessment Report

## Executive Summary

A controlled network security assessment was conducted against a Metasploitable 2 virtual machine in an isolated VirtualBox Host-only network.

The assessment focused on network discovery, service identification, TCP traffic analysis, and HTTP traffic inspection.

## Scope

| Item | Details |
|---|---|
| Analyst machine | Kali Linux |
| Target machine | Metasploitable 2 |
| Target IP | 192.168.182.3 |
| Kali IP | 192.168.182.4 |
| Network | VirtualBox Host-only |
| Tools | Nmap and Wireshark |

## Methodology

1. Verified connectivity between Kali and Metasploitable 2.
2. Performed a basic Nmap scan.
3. Identified open ports and services.
4. Performed service-version detection.
5. Captured traffic using Wireshark.
6. Analyzed TCP and HTTP traffic.
7. Documented observations and recommendations.

## Findings

### Multiple Services Were Exposed

Nmap identified multiple open TCP services on the target machine.

**Impact:** Exposed services increase the attack surface of a system.

**Recommendation:** Disable unnecessary services and restrict access using firewall rules.

### Service Information Was Discoverable

Nmap identified service names and version information.

**Impact:** Service information may help identify outdated or vulnerable software.

**Recommendation:** Keep services updated and limit unnecessary service exposure.

### TCP Traffic Was Observable

Wireshark captured TCP connections between Kali Linux and Metasploitable 2.

**Impact:** Traffic analysis can reveal communication patterns, source and destination addresses, and connection behavior.

**Recommendation:** Monitor network traffic and restrict unauthorized access between systems.

### HTTP Traffic Was Visible

Wireshark captured HTTP traffic involving the target on port 80.

**Impact:** HTTP does not provide encryption. Sensitive data transmitted through HTTP may be exposed on a shared network.

**Recommendation:** Use HTTPS/TLS for sensitive web communication.

## Limitations

- Testing was performed only against an authorized virtual machine.
- The target was intentionally vulnerable for educational purposes.
- No exploitation or brute-force testing was performed.
- The assessment does not represent a complete enterprise security assessment.

## Conclusion

The assessment demonstrated basic network reconnaissance, service identification, TCP traffic analysis, HTTP inspection, and security documentation using Kali Linux, Nmap, Wireshark, and VirtualBox.
