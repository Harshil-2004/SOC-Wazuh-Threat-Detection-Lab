---

# detection-notes/week-2-log-analysis.md

```markdown
# Week 2: Log Analysis and Event Monitoring

## Objective
Understand normal vs suspicious system activity using Windows and Linux logs.

## Windows Log Analysis

### Successful Logon

Event ID:

```text
4624

Wazuh Query:

data.win.system.eventID: 4624

Observation:

Successful logon events were detected from the Windows endpoint and categorized as normal authentication activity.

Failed Logon

Event ID:

4625

Wazuh Query:

data.win.system.eventID: 4625

Observation:

Failed logon events were detected and categorized as suspicious when repeated attempts were observed.

Linux Log Analysis

Linux authentication events were monitored from Kali Linux using SSH and sudo activity.

Useful search terms:

authentication_failure
authentication_success
sshd
sudo
Custom Group

A custom Wazuh group was created for endpoint categorization.

Group name:

Windows-lab
