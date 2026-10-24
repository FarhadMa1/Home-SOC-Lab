# Windows Endpoint Setup

1. Create a Windows 11 VM.
2. Install the Wazuh Agent MSI.
3. Configure manager address during install or via registry/config.
4. Install Sysmon (see sysmon-configuration.md).
5. Restart the Wazuh agent service.

## Verify agent

On the Wazuh manager:

```bash
sudo /var/ossec/bin/agent_control -l
```
