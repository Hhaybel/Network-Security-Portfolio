# Security Incident Investigation — 5-Tuple Analysis

## Overview
This project documents a simulated **network security incident investigation** involving unauthorized command execution, privilege escalation, and data exfiltration.  
The goal was to practice **incident response workflows** and understand how network-level evidence can be used to reconstruct an attacker’s activity.

Using **5-tuple analysis**, packet inspection, and log correlation, the investigation focused on identifying the attacker, understanding the scope of compromise, and proposing remediation steps.

---

## Investigation Focus
- Network Security Monitoring (NSM)
- Incident detection and triage
- 5-tuple traffic analysis
- Packet reconstruction and protocol analysis
- Evidence handling and reporting

---

## Tools & Environment
- **Security Onion** — Intrusion detection and network security monitoring
- **Sguil** — Alert triage and session analysis
- **Wireshark** — Deep packet inspection and TCP stream reconstruction
- **Kibana** — Log correlation and metadata analysis
- **Linux** — Analysis environment and command-line tooling

---

## Key Findings
- Unauthorized command execution was detected through NSM alerts.
- 5-tuple analysis was used to identify the attacking host and affected internal system.
- Packet inspection confirmed privilege escalation and file transfer activity.
- Log correlation validated data exfiltration and helped reconstruct the attack timeline.

---

## Documentation
- **Security_Incident_Investigation_Report.pdf**  
  A full investigation report detailing objectives, observations, conclusions, and remediation recommendations.

---

## Learning Outcomes
- Applied structured incident response methodology
- Improved understanding of network-based attack detection
- Gained hands-on experience correlating alerts, packets, and logs
- Practiced professional security documentation and reporting
