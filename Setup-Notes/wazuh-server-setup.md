# Wazuh Server Setup

## Recommended method

Use the official all-in-one installer on Ubuntu Server:

```bash
curl -sO https://packages.wazuh.com/4.9/wazuh-install.sh
sudo bash wazuh-install.sh -a
```

## After install

1. Access dashboard: https://<wazuh-ip>
2. Note the default credentials printed by the installer.
3. Create an agent enrollment token or use the default method.
4. Open ports: 1514/UDP, 1515/TCP, 55000, 443.

## Verify

```bash
sudo systemctl status wazuh-manager
sudo systemctl status wazuh-indexer
sudo systemctl status wazuh-dashboard
```
