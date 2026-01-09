Incident Response & Network Forensics: Case Study 01
🛡️ Project: Host Isolation & 5-Tuple Analysis
Author: Abel Kolawole
Objective: Investigate a "root-level" compromise and data exfiltration event within a Linux-based infrastructure to identify adversary movement and secure the host.
🔍 Investigation Overview
This case study involves a deep-dive analysis of a security breach where a sensitive file, confidential.txt, was compromised. The investigation follows the full lifecycle of an incident: from initial alert triage to forensic reconstruction and final remediation.
🛠️ Toolset Utilized
• Security Onion (NSM Suite): Centralized platform for network security monitoring.
• Sguil: Used for real-time event triage and correlating high-priority alerts.
• Wireshark: Employed for Deep Packet Inspection (DPI) to reconstruct the TCP stream and identify the specific vulnerability exploited (r3d_dr4g0n).
• Kibana: Utilized for historical log aggregation to track the exfiltration of data via FTP.
• Wormhole.app: Leveraged via an in-VM anonymous browser for end-to-end encrypted evidence transmission, ensuring forensic integrity and host anonymity during the investigation.
📊 Key Investigation Findings
1. Detection: Identified a GPL ATTACK_RESPONSE alert in Sguil, indicating unauthorized command execution.
2. Profiling (The 5-Tuple):
• Source IP: 209.165.200.235 (Port 1234)
• Destination IP: 192.168.0.11 (Port 80)
• Protocol: TCP (6)
3. Forensics: Verified the adversary achieved root-level administrative access and accessed the /home/analyst/ directory.
4. Exfiltration: Confirmed via Kibana that the stolen data was sent to the attacker at 03:53 AM on June 11th.
🛡️ Remediation Strategy
• Logical Isolation: Immediate disconnection of the target host to halt further commands.
• Identity Hardening: Mandatory credential reset for user and root accounts.
• Vulnerability Management: Patching system services to close the exploit vector.
• Egress Filtering: Updating firewall rules to block the malicious 5-tuple signature.
📖 Methodology & References
• Framework: Based on the Cisco CyberOps Associate curriculum for systematic incident handling.
• Community Intelligence: Informed by the r/Cybersecurity community for modern Blue Team tactics.
This project is a part of my Networking and Security Portfolio. All labs are performed in controlled environments for research and educational purposes.
