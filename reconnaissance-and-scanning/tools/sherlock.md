# Sherlock

## Overview
Sherlock is an Open Source Intelligence (OSINT) tool designed to identify the presence of a specific username across a wide range of online platforms. It is commonly used during the reconnaissance phase of security assessments to map a target’s public digital footprint.

Sherlock performs passive reconnaissance and does not exploit vulnerabilities or require authentication.

---

## Primary Use Cases

Sherlock is typically used for:

- Username enumeration across social networks
- Digital footprint analysis
- Supporting social engineering threat modelling
- Initial reconnaissance during penetration testing
- Defensive and investigative security research

---

## How the Tool Works

Many online platforms assign predictable and unique URLs to user profiles. Sherlock takes advantage of this behaviour by:

1. Constructing platform-specific URLs using the target username  
2. Sending HTTP requests to those URLs  
3. Analysing HTTP responses and page content  
4. Determining whether the username exists on each platform

Sherlock supports enumeration across 300+ platforms.

---

## Output and Interpretation

Sherlock output indicates:

- Platforms where the username **exists**
- Platforms where the username **does not exist**
- Platforms that could not be reliably checked

The results provide a snapshot of username presence but do not confirm account ownership or activity.

---

## Limitations

- Dependent on consistent platform URL structures
- Platform changes may cause false positives or negatives
- Results represent a point-in-time snapshot
- Does not validate identity or account legitimacy

---

## Security and Ethical Considerations

Although Sherlock uses publicly available information, improper use may raise privacy concerns or support malicious activity.

This tool should only be used:
- In authorised environments
- For educational, defensive, or investigative purposes
- In accordance with legal and ethical standards

---

## Related Exercises

- [OSINT-Based Username Enumeration](../exercises/sherlock-osint.md)