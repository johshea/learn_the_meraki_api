---
layout: default
title: Lab 7 - Bulk Configuration
---

# 🔹 Lab 7: Bulk Update Switch Ports

## 🎯 Objective:
Update settings across multiple switch ports.

```python
for device in switch_list:
    dashboard.switch.updateDeviceSwitchPort(
        serial=device['serial'],
        portId=1,
        enabled=False
    )
```
