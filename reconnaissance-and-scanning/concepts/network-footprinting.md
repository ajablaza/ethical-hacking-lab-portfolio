# Network Footprinting

Network footprinting focuses on identifying how a target network is structured. It builds upon information gathered from DNS footprinting and expands into understanding routing paths and network boundaries.

---

## Techniques Used

### DNS Footprinting
- Identifying DNS records
- Discovering name servers and host mappings

### Traceroute
Traceroute is used to map the path packets take from the source to a destination. It helps reveal:
- Intermediate routers
- Network latency
- Routing structure

Traceroute leverages the Time To Live (TTL) field in IP packets to identify network hops.

---

## Security Implications

- Exposed routing paths aid attackers in mapping infrastructure
- Network visibility increases reconnaissance effectiveness

---

## Defensive Measures

- Limit ICMP responses where possible
- Harden router configurations
- Apply network segmentation