# Sysmon Configuration

1. Download Sysmon from Microsoft Sysinternals.
2. Use a community config (e.g. SwiftOnSecurity or similar) or a minimal one that captures process creation, network connections, and file events.

Example install:

```powershell
sysmon64.exe -accepteula -i sysmonconfig.xml
```

## Useful Event IDs

- 1: Process creation
- 3: Network connection
- 11: File create
- 22: DNS query

Make sure the Wazuh agent is configured to collect these events.
