# TryHackMe Journal

> 13 rooms completed

---

## Inside a Computer System
**Difficulty:** Easy | **Category:** General

### What I learned
Covered the core components of a computer: CPU, RAM, storage, motherboard. Also went through the boot process from powered off to running OS, including what BIOS/UEFI and the bootloader actually do.

---

## Putting it All Together
**Difficulty:** Easy | **Category:** Web

### What I learned
How everything connects when you load a website. DNS finds the IP, browser sends an HTTP request, server sends back the page, browser renders it. Tied together everything from the previous modules.

---

## How Websites Work
**Difficulty:** Easy | **Category:** Web

### What I learned
How websites are built and delivered. HTML structures the page, JavaScript adds interactivity and runs in the browser. HTML injection is when unsanitized user input gets rendered as HTML. Attackers can inject their own content into the page.

---

## HTTP in Detail
**Difficulty:** Easy | **Category:** Networking

### What I learned
HTTP is how browsers talk to servers. HTTPS encrypts it. GET requests data, POST sends it, PUT updates it, DELETE removes it. Status codes: 200 is good, 404 is not found, 403 is no permission, 500 is server broke. Headers carry extra info like cookies and auth tokens. Cookies keep you logged in since HTTP doesn't remember you. Stolen cookies let attackers log in as you.

---

## DNS in Detail
**Difficulty:** Easy | **Category:** Networking

### What I learned
DNS converts domain names to IP addresses. Query goes through Recursive DNS, Root, TLD, then Authoritative server. Record types: A (IPv4), AAAA (IPv6), CNAME (domain to domain), MX (email routing), TXT (verification and email security like SPF, DKIM, DMARC). DNS is unencrypted by default so it's vulnerable to spoofing.

---

## Extending Your Network
**Difficulty:** Easy | **Category:** Networking

### What I learned
How networks get extended and secured. Port forwarding lets inside devices be reachable from the internet. Firewalls filter traffic by rules: stateful tracks the whole connection, stateless checks individual packets. VPNs encrypt traffic and securely connect networks over the internet. Subnetting divides a network into smaller segments for organization and security.

---

## Packets & Frames
**Difficulty:** Easy | **Category:** Networking

### What I learned
How data gets broken into packets and frames. Frames operate at layer 2 using MAC addresses within a LAN. Packets operate at layer 3 using IP addresses across networks. TCP uses a three-way handshake (SYN, SYN-ACK, ACK) to establish connections and guarantees delivery. UDP is faster but doesn't check if data arrived, used for streaming and gaming.

---

## OSI Model
**Difficulty:** Easy | **Category:** Networking

### What I learned
7 layers describing how data moves across a network. Physical is the raw signal. Data Link uses MAC addresses. Network uses IP addresses. Transport breaks data into chunks. Session manages the connection. Presentation handles encryption. Application is what you interact with. Data gets wrapped going down and unwrapped going up.

---

## Intro to LAN
**Difficulty:** Easy | **Category:** Networking

### What I learned
How LANs are structured. Switches connect devices within a network. Routers connect networks together. ARP maps IP addresses to MAC addresses. DHCP automatically assigns IP addresses to devices.

---

## What is Networking?
**Difficulty:** Easy | **Category:** Networking

### What I learned
The basics of how devices communicate on a network. IP addresses identify devices logically. MAC addresses identify them at the hardware level.

---

## Careers in Cyber
**Difficulty:** Easy | **Category:** Career

### What I learned
Different cyber career paths: red team, blue team, pentesting, forensics, malware analysis. Helped map out where different skills lead.

---

## Defensive Security Intro
**Difficulty:** Easy | **Category:** Defensive Security

### What I learned
The blue team side: SOC roles, threat intelligence, DFIR, and SIEM. Defensive security is about preventing, detecting, and responding to attacks before and after they happen.

---

## Offensive Security Intro
**Difficulty:** Easy | **Category:** Offensive Security

**Tools used:** dirb

### What I learned
How offensive security works by hacking a fake bank site. Used dirb to brute-force hidden directories and found a page that wasn't linked publicly. Core idea: think like an attacker to find what defenders missed.

---
