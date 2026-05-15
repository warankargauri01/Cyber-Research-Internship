# Operation Digital Eye (C0061)

## Campaign Overview
Operation Digital Eye was a cyber campaign conducted during June and July 2024 by suspected China-nexus threat actors targeting business-to-business IT service providers in Southern Europe.

The attackers used Visual Studio Code tunnels, SQL injection attacks, credential dumping, web shells, and lateral movement techniques to maintain access and control over compromised systems.

---

## Threat Actor Association
The campaign is suspected to be associated with People's Republic of China (PRC)-linked threat actors.

The campaign showed overlaps with:
- Operation Soft Cell
- Operation Tainted Love

---

## Timeline
- First Seen: June 2024
- Last Seen: July 2024

---

## Targeted Sectors/Countries
Targets included:
- Business-to-Business IT Service Providers
- Southern Europe

---

## Objectives of Attack
- Unauthorized system access
- Credential theft
- Persistent remote access
- Lateral movement inside victim networks
- Concealing malicious activity

---

## Attack Flow
1. Attackers exploited public-facing applications using SQL injection.
2. Web shells were deployed for persistence.
3. Visual Studio Code tunnels were created for command and control.
4. Credentials were dumped from LSASS memory and SAM database.
5. Threat actors moved laterally using RDP and Pass-the-Hash techniques.
6. Files and indicators were deleted to hide traces.

---

## MITRE ATT&CK Techniques Used

- T1190 – Exploit Public-Facing Application
- T1003.001 – OS Credential Dumping: LSASS Memory
- T1219.001 – Remote Access Tools: IDE Tunneling
- T1505.003 – Web Shell
- T1021.001 – Remote Desktop Protocol
- T1550.002 – Pass the Hash
- T1070.004 – File Deletion

---

## Software Used
- Mimikatz (Credential Dumping)
- PHPsert (Web Shell)
- Ping (Reconnaissance)
- sqlmap (SQL Injection Automation)

---

## Detection Opportunities
- Monitor unusual Visual Studio Code tunnel activity
- Detect suspicious SQL injection attempts
- Monitor LSASS memory access
- Identify unusual RDP movement between systems
- Detect unauthorized Windows services

---

## Defensive Recommendations
- Patch public-facing applications
- Disable unnecessary remote services
- Use Endpoint Detection and Response (EDR)
- Restrict administrative privileges
- Monitor PowerShell and CMD activity
- Implement MFA and credential protection

---

## Indicators of Compromise (IOCs)
- Suspicious Visual Studio Code tunnels
- Unauthorized web shells
- Unusual service names
- SQL injection patterns
- Credential dumping behavior

---

## References
https://attack.mitre.org/campaigns/C0061/
