# Lab Architecture

## Network

Recommended: Host-only or Internal network so attack traffic stays inside the lab.

Example subnet: 192.168.56.0/24 or 10.0.0.0/24

| VM                  | IP (example)   | Role                     |
|---------------------|----------------|--------------------------|
| Wazuh Server        | 192.168.56.10  | SIEM / XDR               |
| Windows Endpoint    | 192.168.56.20  | Victim + Sysmon          |
| Ubuntu Endpoint     | 192.168.56.30  | Linux victim             |
| Kali Linux          | 192.168.56.40  | Attacker                 |

## Resources (minimum)

- Wazuh: 2 CPU / 4-8 GB RAM
- Windows: 2 CPU / 4 GB RAM
- Kali: 2 CPU / 2-4 GB RAM

## Diagram

```
[Kali] --attacks--> [Windows + Sysmon]
                \--> [Ubuntu]
[Windows] --logs--> [Wazuh]
[Ubuntu]  --logs--> [Wazuh]
```
