# Wazuh Search Queries

This file contains important Wazuh queries used during the SOC lab project.

## Windows Successful Logon

```text
data.win.system.eventID: 4624
Windows Failed Logon
data.win.system.eventID: 4625
Windows Agent Filter
agent.name: "Harshil-Windows"
Kali Agent Filter
agent.name: "kali-Agent"
Linux Authentication Failure
rule.groups: authentication_failure
Linux Authentication Success
rule.groups: authentication_success
SSH Events
sshd
SSH Brute Force
sshd brute force
EICAR Test Search
eicar
Sudo Command Execution
sudo
High Severity Alerts
rule.level >= 10
Top Security Rules
rule.description
Alerts by Agent
agent.name
Rule Level Field
rule.level
