# Mimikatz (S0002)

## Name & Type
Mimikatz is a credential dumping and privilege escalation tool.

---

## Description
Mimikatz is a post-exploitation tool used by threat actors to extract credentials from memory, including passwords, hashes, PINs, and Kerberos tickets from Windows systems.

---

## Threat Actor Association
Mimikatz has been used by multiple advanced persistent threat (APT) groups and cybercriminal actors worldwide.

In Operation Digital Eye, attackers used custom implementations of Mimikatz.

---

## Supported Platforms
- Windows

---

## ATT&CK Techniques Used
- T1003.001 – OS Credential Dumping: LSASS Memory
- T1550.002 – Pass the Hash

---

## Execution Method
Threat actors executed Mimikatz using cmd.exe and custom binaries.

---

## Persistence Techniques
Mimikatz itself is mainly used for credential access, though attackers may combine it with persistence mechanisms.

---

## Privilege Escalation
Mimikatz can extract administrator credentials and security tokens for privilege escalation.

---

## Defense Evasion
Custom implementations and renamed executables help evade detection.

---

## Credential Access
Mimikatz targets LSASS memory and SAM database credentials.

---

## Discovery Techniques
Attackers may use system and account discovery before credential dumping.

---

## Lateral Movement
Credentials extracted using Mimikatz can be used for Pass-the-Hash attacks and RDP movement.

---

## Command & Control
Mimikatz itself is not a C2 tool but supports post-exploitation activities.

---

## Exfiltration
Extracted credentials may be transferred to attacker-controlled infrastructure.

---

## Impact Analysis
Successful credential dumping can lead to full domain compromise and unauthorized access to sensitive systems.

---

## Indicators of Compromise (IOCs)
- Suspicious LSASS access
- Unusual cmd.exe execution
- Credential dumping behavior
- Unauthorized SAM access

---

## Detection & Mitigation
- Monitor LSASS memory access
- Enable Credential Guard
- Restrict administrative privileges
- Use Endpoint Detection & Response (EDR)

---

## References
https://attack.mitre.org/software/S0002/
