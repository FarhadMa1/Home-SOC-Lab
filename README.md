# Home SOC Lab

## Overview

This repository documents a home Security Operations Center (SOC) lab built for practicing blue-team skills.

Typical stack:
- **Hypervisor**: Oracle VirtualBox
- **SIEM/XDR**: Wazuh (Manager + Dashboard)
- **Endpoints**: Windows 11 + Sysmon, Ubuntu Server
- **Attacker**: Kali Linux (optional)
- Isolated internal network

## Goals
- Deploy Wazuh and ingest logs
- Collect rich Windows telemetry with Sysmon
- Simulate attacks and investigate alerts
- Write structured incident reports
- Practice threat hunting and MITRE ATT&CK mapping

## Repository Structure

```
Home-SOC-Lab/
├── README.md
├── Architecture/
│   └── architecture.md
├── Setup-Notes/
│   ├── wazuh-server-setup.md
│   ├── windows-endpoint-setup.md
│   └── sysmon-configuration.md
├── Detection-Scenarios/
│   └── 01-example-scenario/
│       └── report.md
└── References/
    └── references.md
```

## Lab Status

| Component              | Status      |
|------------------------|-------------|
| VirtualBox network     | To do       |
| Wazuh Server           | To do       |
| Windows endpoint       | To do       |
| Sysmon                 | To do       |
| Attack simulations     | To do       |
| Detection reports      | To do       |

## Disclaimer

For educational and defensive security practice only. Keep the lab isolated.
