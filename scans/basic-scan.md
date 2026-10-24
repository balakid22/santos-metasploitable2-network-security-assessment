# Basic Nmap Scan

## Target

Metasploitable 2

Target IP: `192.168.182.3`

## Result

The host was up and multiple TCP ports were open.

| Port | Service |
|---|---|
| 21/tcp | FTP |
| 22/tcp | SSH |
| 23/tcp | Telnet |
| 25/tcp | SMTP |
| 53/tcp | DNS |
| 80/tcp | HTTP |
| 111/tcp | RPCBind |
| 139/tcp | NetBIOS-SSN |
| 445/tcp | Microsoft-DS |
| 512/tcp | Exec |
| 513/tcp | Login |
| 514/tcp | Shell |
| 1099/tcp | RMI Registry |
| 1524/tcp | Ingreslock |
| 2049/tcp | NFS |
| 2121/tcp | FTP Proxy |
| 3306/tcp | MySQL |
| 5432/tcp | PostgreSQL |
| 5900/tcp | VNC |
| 6000/tcp | X11 |
| 6667/tcp | IRC |
| 8009/tcp | AJP13 |
| 8180/tcp | HTTP Proxy |

## Observation

The target exposed multiple network services, creating a larger attack surface within the intentionally vulnerable lab environment.

No exploitation was performed.
