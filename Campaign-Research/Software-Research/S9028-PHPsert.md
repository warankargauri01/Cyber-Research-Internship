# PHPsert (S9028)

## Name & Type

PHPsert is a PHP-based web shell used for remote access and persistence.

---

## Description

PHPsert is a malicious PHP web shell that allows threat actors to execute commands, maintain persistence, and control compromised web servers remotely.

During Operation Digital Eye, attackers deployed PHPsert to maintain unauthorized access to targeted systems.

---

## Threat Actor Association

PHPsert has been associated with threat actors involved in Operation Digital Eye.

---

## Supported Platforms

- Web Servers
- Linux
- Windows Servers running PHP

---

## ATT&CK Techniques Used

- T1505.003 – Server Software Component: Web Shell

---

## Execution Method

Threat actors deploy PHPsert onto compromised web servers and execute commands remotely through web requests.

---

## Persistence Techniques

PHPsert maintains persistent access by remaining hidden inside compromised web server directories.

---

## Privilege Escalation

Attackers may combine PHPsert with other tools to escalate privileges after initial access.

---

## Defense Evasion

PHPsert can hide within legitimate web server files and directories to avoid detection.

---

## Credential Access

Threat actors may use PHPsert to access sensitive files and credentials stored on servers.

---

## Discovery Techniques

Attackers may use PHPsert to gather information about the compromised system and network.

---

## Lateral Movement

PHPsert may assist attackers in moving across systems after gaining server access.

---

## Command & Control

PHPsert allows remote command execution and communication with attacker-controlled infrastructure.

---

## Exfiltration

Sensitive data from compromised servers may be transferred through the web shell.

---

## Impact Analysis

PHPsert can provide persistent unauthorized access, enable remote control, and support further attacks inside victim environments.

---

## Indicators of Compromise (IOCs)

- Suspicious PHP files
- Unauthorized web shell activity
- Unusual web requests
- Unknown server-side scripts

---

## Detection & Mitigation

- Monitor web server directories
- Detect suspicious PHP activity
- Use Web Application Firewalls (WAF)
- Restrict file upload permissions
- Perform regular server scans

---

## References

https://attack.mitre.org/software/S9028/
