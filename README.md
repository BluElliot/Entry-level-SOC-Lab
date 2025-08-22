# Entry-level-SOC-Lab
A entry-level SOC lab that uses Splunk to detect attacks and demonstrates skills in log collection, dashboards, and alerts.

## Overview
This a Security Operations Center (SOC) lab using **Splunk Enterprise** as the SIEM.  
The goal is to practice and showcase entry-level SOC skills:
- Detecting password spray attacks
- Triage of phishing emails
- Detecting malware (EICAR test file)
- Responding to incidents

## Lab Topology
- **Ubuntu Server** → Splunk Enterprise (SIEM, dashboards, alerts)
- **Windows Server (AD/DC)** → Authentication logs
- **Windows Client (Target)** → User endpoint
- **Kali Linux (Attacker)** → Simulates password spray, phishing, malware

## Tools & Technologies
- VMware Workstation
- Splunk Enterprise (Free 500MB/day license)
- Splunk Universal Forwarder
- Sysmon, auditd, EICAR test file

## Example Scenarios
- **Password Spray** → Detect via EventCode=4625 SPL query
- **Phishing Triage** → Analyze headers/logs
- **Malware (EICAR)** → Trigger AV alert, detect in Splunk

## Repository Structure
- `docs/` → Project chapters
- `configs/` → Config files (Sysmon, Splunk inputs, auditd)
- `queries/` → SPL queries
- `reports/` → Case studies & metrics
- `screenshots/` → Visuals of dashboards/alerts
