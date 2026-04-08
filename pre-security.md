# TryHackMe Journal

> 11 rooms completed

---

## How Websites Work
**Difficulty:** Easy  |  **Category:** Web

### What I learned
Learned how websites are built and delivered. HTML structures the page, JavaScript adds interactivity and runs in the browser. HTML injection is a vulnerability where unsanitized user input gets rendered as HTML — attackers can inject their own content into the page.

---

## HTTP in Detail
**Difficulty:** Easy  |  **Category:** Networking

### What I learned
HTTP is how browsers communicate with web servers. HTTPS adds TLS encryption. Methods: GET (request data), POST (send data), PUT (update), DELETE (remove). Status codes: 200 OK, 301 redirect, 404 not found, 403 forbidden, 500 server error. Headers carry metadata like browser info, auth tokens, and cookies. Cookies keep you logged in since HTTP is stateless — server stores a session ID in your browser. Stolen cookies = session hijacking.

---

## DNS in Detail
**Difficulty:** Easy  |  **Category:** Networking

### What I learned
DNS converts domain names to IP addresses. Query goes through Recursive DNS, Root, TLD, then Authoritative server. Record types: A (IPv4), AAAA (IPv6), CNAME (domain to domain), MX (email routing), TXT (verification and email security like SPF, DKIM, DMARC). DNS is unencrypted by default making it vulnerable to spoofing.

---

## Extending Your Network
**Difficulty:** Easy  |  **Category:** Networking

### What I learned
Learned how networks get extended and secured. Port forwarding lets inside devices be reachable from the internet. Firewalls filter traffic by rules — stateful tracks the whole connection, stateless checks individual packets. VPNs securely connect networks over the internet and encrypt traffic. Subnetting divides a network into smaller segments for organization and security.

---

## Packets & Frames
**Difficulty:** Easy  |  **Category:** Networking

### What I learned
Learned how data is broken into packets and frames. Frames operate at layer 2 using MAC addresses within a LAN, packets operate at layer 3 using IP addresses across networks. TCP uses a three-way handshake (SYN, SYN-ACK, ACK) to establish connections and guarantees delivery. UDP is faster but doesn't check if data arrived — used for streaming and gaming.

---

## OSI Model
**Difficulty:** Easy  |  **Category:** Networking

### What I learned
Learned the 7 OSI layers and how data travels through them. Each layer has a specific job — Physical handles raw signals, Data Link uses MAC addresses, Network uses IP addresses, Transport breaks data into chunks, Session manages connections, Presentation handles encryption, Application is what the user interacts with. Data gets encapsulated going down and decapsulated going up.

### Notes
Mnemonic: Please Do Not Throw Sausage Pizza Away

---

## Intro to LAN
**Difficulty:** Easy  |  **Category:** Networking

### What I learned
Learned how LANs are structured. Switches connect devices within a network, routers connect networks together. ARP maps IP addresses to MAC addresses, DHCP automatically assigns IP addresses to devices.

---

## What is Networking?
**Difficulty:** Easy  |  **Category:** Networking

### What I learned
Learned the basics of how devices communicate on a network. IP addresses identify devices logically, MAC addresses identify them at the hardware level.

---

## Careers in Cyber
**Difficulty:** Easy  |  **Category:** Career

### What I learned
Explored different cyber career paths — red team, blue team, pentesting, forensics, malware analysis. Helped map out where different skills lead.

### Notes
Career quiz result: Penetration Tester

---

## Defensive Security Intro
**Difficulty:** Easy  |  **Category:** Defensive Security

### What I learned
Covered the blue team side — SOC roles, threat intelligence, DFIR, and SIEM. Defensive security is about preventing, detecting, and responding to attacks before and after they happen.

---

## Offensive Security Intro
**Difficulty:** Easy  |  **Category:** Offensive Security

**Tools used:** dirb

### What I learned
Learned how offensive security works by hacking a fake bank site. Used dirb to brute-force hidden directories and found a page that wasn't linked publicly. Core idea: think like an attacker to find what defenders missed.

---
