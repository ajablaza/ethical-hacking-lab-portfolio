# Nmap (Network Mapper)

Nmap (Network Mapper) is an open-source network scanning tool widely used for network discovery, host enumeration, and port scanning. It enables security professionals and attackers alike to identify active hosts, open ports, running services, and network filtering mechanisms.

In this project, Nmap was used during the reconnaissance and scanning phase to assess the visibility and exposure of an OWASP Broken Web Application hosted on an internal network. Multiple scan types were executed to demonstrate how different probing techniques can reveal varying levels of information depending on firewall rules, host configurations, and protocol behavior.

## Key Capabilities Demonstrated

- Host discovery using UDP and ICMP-based probes
- Detection of live hosts within a subnet
- Identification of open, filtered, and closed ports
- Comparison of TCP scanning techniques and their visibility
- Enumeration of UDP services

## Scan Techniques Used

### Host Discovery
- **UDP Ping Scan (`-PU`)**  
  Used to determine whether a host is active by sending UDP probes.

- **ICMP Timestamp Ping (`-PP`)**  
  Used to retrieve timestamp information from the target, which may reveal system time and responsiveness.

### TCP Scanning Techniques
- **TCP Full Connection Scan (`-sT`)**  
  Performs a complete TCP handshake and is highly reliable, but noisy.

- **TCP SYN (Stealth) Scan (`-sS`)**  
  Sends SYN packets without completing the handshake, making it more discreet.

- **TCP Xmas Scan (`-sX`)**  
  Sends packets with unusual flag combinations to infer port states through responses or lack thereof.

- **TCP ACK Scan (`-sA`)**  
  Used to determine whether ports are filtered by a firewall rather than open or closed.

### UDP Scanning
- **UDP Scan (`-sU`)**  
  Used to identify exposed UDP services, which are often overlooked due to slower scan times and limited responses.

## Security Relevance

Understanding how different Nmap scan types behave helps security practitioners:
- Identify unintended exposure of services
- Validate firewall and filtering rules
- Assess how an attacker may enumerate network resources
- Improve defensive monitoring and intrusion detection strategies

## Related Exercise

All commands, screenshots, and analysis for Nmap usage in this project are documented in:

[Network Discovery and Port Scanning](../exercises/network-discovery-and-port-scanning.md)

➡️ **`reconnaissance-and-scanning/network-discovery-and-port-scanning.md`**
