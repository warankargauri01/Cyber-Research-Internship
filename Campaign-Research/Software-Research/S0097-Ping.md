# Ping (S0097)

## Name & Type

Ping is a network utility tool used for connectivity testing and reconnaissance.

---

## Description

Ping is a legitimate network diagnostic tool used to test connectivity between systems.

Threat actors often abuse Ping during cyber operations to identify active hosts, perform reconnaissance, and map network environments.

During Operation Digital Eye, attackers used Ping for reconnaissance activities inside targeted networks.

---

## Threat Actor Association

Ping has been used by multiple threat actors and cybercriminal groups during network reconnaissance operations.

In Operation Digital Eye, attackers used Ping to identify reachable systems.

---

## Supported Platforms

- Windows
- Linux
- macOS

---

## ATT&CK Techniques Used

- T1018 – Remote System Discovery

---

## Execution Method

Threat actors execute Ping through command-line interfaces to test network connectivity and discover remote systems.

---

## Persistence Techniques

Ping itself does not provide persistence mechanisms.

---

## Privilege Escalation

Ping is generally not used for privilege escalation.

---

## Defense Evasion

Attackers may use legitimate system tools like Ping to blend malicious activity with normal administrative behavior.

---

## Credential Access

Ping does not directly perform credential access.

---

## Discovery Techniques

Ping is used to identify live hosts and available systems within a network.

---

## Lateral Movement

Ping may assist attackers during lateral movement planning by identifying accessible systems.

---

## Command & Control

Ping itself is not a command-and-control tool.

---

## Exfiltration

Ping is generally not used for data exfiltration.

---

## Impact Analysis

Reconnaissance using Ping helps attackers understand network structure and identify targets for further attacks.

---

## Indicators of Compromise (IOCs)

- Unusual Ping sweeps
- Repeated ICMP requests
- Reconnaissance activity from unauthorized systems

---

## Detection & Mitigation

- Monitor excessive ICMP traffic
- Restrict unnecessary Ping usage
- Use network monitoring tools
- Detect abnormal reconnaissance behavior

---

## References

https://attack.mitre.org/software/S0097/
