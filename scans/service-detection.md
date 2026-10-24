# Nmap Service Detection

## Target

Metasploitable 2

Target IP: `192.168.182.3`

## Identified Services

| Port | Service and Version |
|---|---|
| 21/tcp | vsftpd 2.3.4 |
| 22/tcp | OpenSSH 4.7p1 Debian |
| 23/tcp | Linux telnetd |
| 25/tcp | Postfix smtpd |
| 53/tcp | ISC BIND 9.4.2 |
| 80/tcp | Apache httpd 2.2.8 |
| 139/tcp | Samba smbd |
| 445/tcp | Samba smbd |
| 512/tcp | netkit-rsh rexecd |
| 513/tcp | rlogin |
| 514/tcp | rshd |
| 1099/tcp | GNU Classpath RMI Registry |
| 1524/tcp | Metasploitable root shell |
| 2049/tcp | NFS |
| 2121/tcp | ProFTPD 1.3.1 |
| 3306/tcp | MySQL 5.0.51a |
| 5432/tcp | PostgreSQL 8.3.0–8.3.7 |
| 5900/tcp | VNC protocol 3.3 |
| 6000/tcp | X11 |
| 6667/tcp | UnrealIRCd |
| 8009/tcp | Apache JServ |
| 8180/tcp | Apache Tomcat/Coyote JSP engine |

## Observation

Nmap was able to identify service names and version information from the exposed ports.

This information could help a security analyst identify outdated or unnecessary services.

No exploitation was performed.
