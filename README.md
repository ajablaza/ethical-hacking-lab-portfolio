# Ethical Hacking & Web Application Security Lab Portfolio

This repository documents my practical learning in ethical hacking and
web application security, conducted entirely within **controlled, isolated
lab environments**.

All content has been sanitised and rewritten for educational and
portfolio purposes. No real-world systems, credentials, or sensitive
data are included.

---

## Lab Environment Overview

All labs in this repository were performed on **internal virtual networks**
designed to simulate realistic enterprise-style environments while remaining
fully isolated from the internet and external systems.

The same network topology and virtual machines were used consistently
throughout the project to allow for repeatable testing and comparative learning.

---

## Internal Network 1 – `intnet`

This network represents an internal corporate environment containing
user workstations, servers, and perimeter security controls.

### Machines:
- **Kali Linux**
  - Used as the attacker / security testing workstation
  - Tools included Nmap, Burp Suite, Metasploit, and manual testing

- **Windows 10**
  - Represents a standard internal user endpoint
  - Used for traffic observation, credential handling, and pivoting scenarios

- **Ubuntu Server**
  - Hosts a deliberately vulnerable web application
  - Used for web application security testing (e.g. OWASP Broken Web App)

- **pfSense Firewall**
  - Acts as the network perimeter and traffic control point
  - Used to observe how firewall placement and rules impact attack surfaces

---

## Internal Network 2 – `intnet2`

This secondary internal network is used to simulate lateral movement and
interaction with legacy or insecure systems.

### Machines:
- **Windows 10**
  - Dual-homed system with network interfaces on both `intnet` and `intnet2`
  - Used to explore trust boundaries and network segmentation concepts

- **Metasploitable**
  - Intentionally vulnerable Linux system
  - Used for service enumeration, exploitation testing, and post-compromise analysis

---

## Scope & Ethics

All testing documented in this repository:
- Was performed in **isolated lab environments**
- Targeted **intentionally vulnerable systems**
- Followed ethical hacking principles
- Focused equally on **attack methodology and defensive mitigation**

This repository is intended to demonstrate:
- Practical security testing methodology
- An attacker mindset balanced with defensive awareness
- Progressive learning across multiple lab scenarios

