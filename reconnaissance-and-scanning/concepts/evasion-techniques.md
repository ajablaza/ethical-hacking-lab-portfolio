# IDS and Firewall Evasion Techniques

Attackers may attempt to bypass Intrusion Detection Systems (IDS) and firewalls during reconnaissance and scanning activities.

---

## Common Evasion Techniques

### Packet Fragmentation
Breaking packets into smaller fragments to evade signature-based detection.

### Source Port Manipulation
Using trusted source ports (e.g. 80, 443, 53) to bypass filters.

### IP Address Spoofing
Altering packet headers to mask the true source IP address.

### Firewalking
Firewalking is a technique used to determine which packets can traverse a firewall by analysing responses to probe packets. It builds upon traceroute behaviour to infer firewall rules.

---

## Security Implications

- Misconfigured firewalls are highly vulnerable
- Evasion techniques complicate monitoring and detection

---

## Defensive Measures

- Stateful firewall configurations
- Deep packet inspection
- Correlation-based IDS rules