---
layout: default
title: Lab 5 - Automation Scripts
---

# 🔹 Lab 5: Automate Getting Devices by Network

## 🎯 Objective:
Use Python to pull all devices per network in your organization.

```python
org_id = 'your_org_id'
networks = dashboard.organizations.getOrganizationNetworks(org_id)

for net in networks:
    devices = dashboard.networks.getNetworkDevices(net['id'])
    print(f"Network {net['name']} has {len(devices)} devices.")
```
