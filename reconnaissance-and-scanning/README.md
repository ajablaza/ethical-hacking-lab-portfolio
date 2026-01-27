# Reconnaissance and Scanning

This section documents the reconnaissance and scanning phase of security testing conducted within a controlled lab environment. The objective of this phase is to identify exposed information, services, and potential attack surfaces before any exploitation activities occur.

The techniques demonstrated here reflect how attackers and penetration testers gather intelligence, as well as how defenders can reduce visibility and information leakage.

---

## Objectives

- Identify publicly and internally exposed information
- Discover live hosts, open ports, and running services
- Enumerate technologies used by target systems
- Collect information that could support later attack stages

---

## Lab Context

All activities in this section were performed against systems hosted in isolated internal networks:

### Networks Used
- **intnet**  
  - Kali Linux (attacker)
  - Ubuntu Server hosting OWASP Broken Web Application (target)

These environments allow safe testing of reconnaissance and scanning techniques without external exposure.

---

## Techniques Covered

### Footprinting & OSINT
Techniques focused on gathering information with minimal interaction:

- Username and account discovery using **Sherlock**
- Technology and application identification
- Identifying publicly accessible information relevant to targets

---

### Website Enumeration & Mirroring
Techniques used to understand web application structure and exposed resources:

- Website mirroring using **HTTrack**
- Website mirroring using **Teleport Pro**
- Reviewing mirrored content for hidden paths, files, and exposed assets

---

### Banner Grabbing & Service Identification
Methods used to identify running services and software versions:

- Banner grabbing using **OWASP ZAP**
- Manual inspection of HTTP responses and headers

---

### Network & Port Scanning
Active probing to identify reachable systems and exposed services:

- Host discovery and port scanning using **Nmap**
- Identification of open ports, protocols, and running services
- Foundational enumeration to support further testing phases

---

## Security Perspective

From a defensive standpoint, this phase highlights:

- The risks of exposed services and verbose banners
- The importance of proper firewall segmentation
- How publicly accessible information can aid attackers
- The need for service hardening and minimising attack surface

---

## Ethical Considerations

All techniques demonstrated were executed:

- In controlled lab environments
- Against systems explicitly designed or authorised for testing
- For educational and defensive learning purposes only

No unauthorised systems were targeted.

---

## Related Sections

Detailed walkthroughs, outputs, and tool-specific documentation are available in subdirectories under this section.
