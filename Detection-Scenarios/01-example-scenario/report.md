# Example Detection Scenario

## Title
Local Group Discovery

## MITRE
- Tactic: Discovery
- Technique: T1069.001 - Local Group Membership Discovery

## Simulation
On the Windows endpoint:

```cmd
net localgroup administrators
```

## Expected Detection
- Sysmon Event ID 1 for net.exe
- Wazuh rule that matches process creation with "net.exe" and group-related arguments

## Investigation Steps
1. Search in Wazuh Threat Hunting for the process.
2. Check parent process.
3. Map to MITRE.
4. Write findings.

## Notes
Replace this with your real findings and screenshots.
