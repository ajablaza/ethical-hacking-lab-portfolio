# OWASP ZAP (Zed Attack Proxy)

## Overview
OWASP ZAP (Zed Attack Proxy) is a web application security testing tool commonly used for intercepting, inspecting, and modifying HTTP and HTTPS traffic between a client and a web application.

ZAP is frequently used during reconnaissance and testing phases to identify exposed metadata, application behaviour, and potential security weaknesses.

---

## Primary Use Cases

OWASP ZAP is commonly used for:

- Intercepting HTTP/HTTPS requests and responses
- Banner grabbing and header inspection
- Web application enumeration
- Vulnerability discovery and testing
- Security assessment and learning environments

---

## How the Tool Works

ZAP operates as a proxy between a client (such as a browser) and a web server.

When configured:
1. Client requests are routed through ZAP
2. ZAP intercepts requests and responses
3. HTTP headers and body content can be inspected
4. Application behaviour can be analysed in real time

This allows detailed visibility into how applications communicate over the network.

---

## Banner Grabbing with ZAP

Banner grabbing involves examining HTTP response headers to identify:

- Server type
- Server version
- Framework or platform details
- Application metadata

This information is often unintentionally exposed by web servers and can provide valuable insight to attackers.

---

## Limitations

- Banner information may be deliberately hidden or spoofed
- Not all servers disclose version details
- Requires proper proxy configuration

---

## Security and Ethical Considerations

OWASP ZAP should only be used in authorised environments such as:
- Controlled lab networks
- Deliberately vulnerable applications
- Systems with explicit permission for testing

Improper use may violate privacy or legal boundaries.

---

## Related Exercises

- [Banner Grabbing Using OWASP ZAP](../exercises/zaproxy-banner-grabbing.md)