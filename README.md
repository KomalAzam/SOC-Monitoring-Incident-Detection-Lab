# SOC Monitoring & Incident Detection Lab

A hands-on SOC and Blue Team project focused on security monitoring, alert detection, incident investigation, and MITRE ATT&CK mapping.

## Project Overview

This project was developed as a practical cybersecurity portfolio project to demonstrate hands-on experience with Security Operations Center (SOC) monitoring and Blue Team activities.

The lab involved configuring a Wazuh Manager on Ubuntu, monitoring a Windows endpoint using the Wazuh Agent, generating controlled security events, investigating alerts, and documenting findings.

## Lab Environment

- Windows 11 Pro — Endpoint / Wazuh Agent
- Ubuntu — Wazuh Manager
- VirtualBox — Virtualization
- Kali Linux — Network scanning
- Wazuh — SIEM and security monitoring
- Suricata — IDS monitoring
- Nmap — Network reconnaissance
- Wireshark — Network traffic analysis
- MITRE ATT&CK — Technique mapping

## Security Scenarios Tested

### 1. SSH Brute-Force Detection
- Performed controlled SSH authentication attempts.
- Monitored authentication failures using Wazuh.
- Investigated Wazuh Rule 5712.
- Mapped the activity to MITRE ATT&CK T1110 — Brute Force.

### 2. Network Scanning
- Performed controlled Nmap scanning against the lab environment.
- Used:
  `nmap -sS -T3`
- Analyzed the discovered network services.

### 3. File Integrity Monitoring
- Configured File Integrity Monitoring on the Windows endpoint.
- Created a test file using PowerShell.
- Observed the resulting Wazuh FIM alert.

### 4. Suricata IDS Monitoring
- Used Suricata on the Windows host for IDS monitoring.
- Integrated security monitoring with Wazuh.
- Investigated the generated Suricata alert.

### 5. Windows Failed Logon Detection
- Analyzed Windows Event ID 4625.
- Investigated failed authentication activity and related event information.

## Incident Investigation Process

The project followed a basic SOC investigation workflow:

1. Detect the security alert
2. Validate the alert
3. Identify the affected system and relevant event information
4. Analyze logs and activity
5. Determine the nature of the activity
6. Map confirmed activity to MITRE ATT&CK where applicable
7. Document findings and evidence

## Skills Demonstrated

- SOC Monitoring
- Log Analysis
- Security Alert Investigation
- Incident Investigation
- File Integrity Monitoring
- Network Reconnaissance
- IDS Monitoring
- Windows Event Analysis
- MITRE ATT&CK Mapping
- Wazuh
- Suricata
- Nmap
- Wireshark
- Linux and Windows
- Virtual Machine Administration

## Future Improvements

- Add additional Windows security event detections
- Develop custom Wazuh detection rules
- Integrate additional endpoint telemetry
- Expand incident response scenarios
- Improve automated alert enrichment and investigation workflows

## Disclaimer

This project was conducted in a controlled lab environment for educational and portfolio purposes.
