# SOC Operations & Threat Detection Lab using Wazuh

## Project Overview

This project demonstrates the implementation of a Security Operations Center (SOC) lab using Wazuh SIEM/XDR. The lab was designed to monitor endpoints, collect logs, analyze security events, simulate attack scenarios, and create professional SOC dashboards.

The project was completed as part of the CFSS Global Internship Program 2026 under the domain of SOC Analyst & Blue Teaming.

## Internship Details

**Program:** CFSS Global Internship Program 2026  
**Domain:** SOC Analyst & Blue Teaming  
**Project Title:** SOC Operations & Threat Detection Mastery  
**Duration:** 4 Weeks  
**Submitted By:** Harshil Miteshkumar Barot  

## Tools and Technologies Used

- Wazuh SIEM/XDR
- Wazuh Manager
- Wazuh Agent
- Wazuh Dashboard / OpenSearch Dashboards
- Windows 11
- Kali Linux
- VirtualBox
- Hydra
- EICAR Test File

## Lab Architecture

The SOC lab was built using a Wazuh Manager deployed in a virtualized environment. Windows and Kali Linux endpoints were connected as Wazuh agents. These agents forwarded logs and security events to the Wazuh Manager, where events were analyzed and visualized through the dashboard.

```text
Windows 11 Agent ─────┐
                      │
                      v
                 Wazuh Manager
                      │
                      v
                 Wazuh Dashboard
                      ^
                      │
Kali Linux Agent ─────┘

## Weekly Project Summary

### Week 1: Lab Architecture & Deployment

**Objective:** Build a basic Security Operations Center lab environment.

**Work Completed:**
- Installed and configured Oracle VirtualBox for virtualization.
- Deployed Wazuh Manager using the Wazuh OVA image.
- Accessed the Wazuh Dashboard through the manager IP address.
- Installed Wazuh Agent on the Windows endpoint.
- Installed Wazuh Agent on Kali Linux.
- Verified that both agents appeared as active in the Wazuh Dashboard.

**Deliverable:**
- Wazuh Dashboard screenshot showing active agents.

---

### Week 2: Log Analysis & Event Monitoring

**Objective:** Understand normal and suspicious log activity.

**Work Completed:**
- Monitored Windows Event Logs using Wazuh.
- Filtered Windows successful logon events using Event ID 4624.
- Filtered Windows failed logon events using Event ID 4625.
- Monitored Kali Linux authentication logs.
- Created a custom Wazuh group named `Windows-lab`.
- Collected the top security events triggered during the monitoring period.

**Deliverable:**
- Top 10 security events table.
- Screenshots of successful and failed logon events.

---

### Week 3: Attack Simulation & Detection

**Objective:** Simulate attacker-like activity and observe Wazuh detection.

**Work Completed:**
- Performed a controlled SSH brute-force simulation using Hydra in a local lab environment.
- Verified brute-force detection in Wazuh with a Level 10 alert.
- Used the EICAR test string for safe malware simulation.
- Monitored privileged command execution such as sudo/root activity.
- Reviewed Wazuh alerts generated during the simulations.

**Deliverable:**
- Screenshots of brute-force detection, EICAR simulation, and command monitoring alerts.

---

### Week 4: Dashboarding & Final Reporting

**Objective:** Present SOC monitoring data in a professional format.

**Work Completed:**
- Created custom visualizations in Wazuh/OpenSearch Dashboards.
- Built a custom dashboard named `Harshil's Dashboard`.
- Added a bar chart for Total Alerts per Day.
- Added a donut chart for Top 5 Security Rules Triggered.
- Added a data table for Agent Status Overview.
- Prepared the final internship project report in PDF format.

**Deliverable:**
- Final PDF report.
- GitHub repository with configuration notes and project documentation.

Key Detection Areas
Windows successful logon detection
Windows failed logon detection
Linux SSH authentication failure
SSH brute-force detection
Compliance/SCA monitoring
EICAR malware simulation
Privileged command monitoring
Agent status monitoring
