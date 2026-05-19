  # Cybersecurity Home Lab Portfolio

## About
Self-taught security practitioner building practical skills through home lab simulations. Each lab covers a real-world attack scenario; from initial access to detection, investigation, and incident response.

**Tools & Technologies:**  
`Kali Linux` `Metasploit` `Nmap` `Wireshark` `Splunk` `Sysmon` `VirtualBox` `Python`

**Frameworks:**  
`NIST SP 800-61` `MITRE ATT&CK` `PICERL`

---
## SOC Labs - Detection and Incident Response
Simulated attacks detected and investigated using Splunk + Sysmon, documented following the **NIST SP 800-61** Incident Handling Framework.
| # | Lab | Attack Type | Tools | Severity |
|---|-----|-------------|-------|----------|
| 01 | [Meterpreter C2 via Social Engineering](./soc-labs/lab-01-meterpreter-c2/INCIDENT_REPORT.md) | Reverse Shell | Metasploit, Splunk, Sysmon, Wireshark | Critical |

## Pentest Labs *(Comming soon)*
| # | Lab | Target | Technique | CVE |
|---|-----|--------|-----------|-----|
| - | - | - | - | - |

---
## Lab Environment
All labs run in an isolated virtual network.

```
┌─────────────────────────────────────────────┐
│           VirtualBox Host-Only Network      │
│              192.168.56.0/24                │
│                                             │
│  ┌───────────────┐     ┌───────────────┐    │
│  │  Kali Linux   │───▶│  Windows 11   │    │
│  │ 192.168.56.101│     │ 192.168.56.102│    │
│  │  (Attacker)   │     │   (Victim)    │    │
│  └───────────────┘     └───────────────┘    │
│                               │             │
│                        Sysmon + Splunk UF   │
│                               │             │
│                    ┌──────────▼──────────┐  │
│                    │   Host Machine      │  │
│                    │  Splunk Enterprise  │  │
│                    │   (SIEM / SOC)      │  │
│                    └─────────────────────┘  │
└─────────────────────────────────────────────┘
```

## Connect
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=flat&logo=linkedin)](https://linkedin.com/in/luisgabriel-delfinpaulin)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-Profile-red?style=flat&logo=tryhackme)](https://tryhackme.com/p/luisgabrieldp)
