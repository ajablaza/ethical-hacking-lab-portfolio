# Website Enumeration and Mirroring

Website enumeration involves analysing a target web application to understand its structure, technologies, and exposed content. One common technique is website mirroring, which creates a local copy of the site for offline analysis.

---

## Website Enumeration Objectives

- Identify hidden directories and files
- Analyse application structure
- Locate exposed configuration or backup files
- Support vulnerability discovery

---

## Website Mirroring

Website mirroring replicates the contents of a target website locally.

Advantages:
- Enables offline review
- Reveals hidden or linked resources
- Supports wordlist generation

Tools such as HTTrack and Teleport Pro were used to perform mirroring activities.

---

## Security Implications

- Excessive exposure of web content increases attack surface
- Forgotten files and directories may leak sensitive information
- Poor access control enables enumeration

---

## Defensive Considerations

- Restrict unnecessary files and directories
- Implement access controls
- Regularly audit web content