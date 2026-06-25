---

# detection-notes/week-3-attack-simulation.md

```markdown
# Week 3: Attack Simulation and Detection

## Objective
Simulate attacker-like behavior in a controlled lab and verify detection in Wazuh.

## 1. Brute Force Simulation

A controlled SSH brute-force simulation was performed using Hydra against the local Kali SSH service.

Purpose:

- Generate repeated authentication failure logs.
- Verify Wazuh brute-force detection.
- Understand how brute-force behavior appears in SIEM alerts.

Detection:

- Rule Description: sshd: brute force trying to get access to the system
- Rule ID: 5763
- Rule Level: 10
- MITRE Technique: T1110

## 2. Malware Simulation

A safe EICAR antivirus test string was used to simulate malware detection behavior.

Important Note:

EICAR is not real malware. It is a harmless test file used to validate antivirus and security monitoring detection.

## 3. Command Monitoring

Privileged command execution was monitored using Linux sudo/root activity.

Detection:

- Rule Description: Successful sudo to ROOT executed
- Rule ID: 5402

## Outcome

Wazuh successfully detected authentication failure events, brute-force behavior, EICAR-related test activity, and privileged command execution
