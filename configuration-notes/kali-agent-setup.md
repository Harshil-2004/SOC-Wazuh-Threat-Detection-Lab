
---

# configuration-notes/kali-agent-setup.md

```markdown
# Kali Linux Agent Setup

## Objective
Install and configure the Wazuh Agent on Kali Linux for Linux log monitoring.

## Steps Performed

1. Installed the Wazuh Agent package on Kali Linux.
2. Configured the Wazuh Manager IP address.
3. Enabled the Wazuh Agent service.
4. Started the Wazuh Agent service.
5. Verified the agent status using systemctl.
6. Confirmed that the Kali agent appeared active in the Wazuh Dashboard.

## Service Verification

```bash
sudo systemctl status wazuh-agent
