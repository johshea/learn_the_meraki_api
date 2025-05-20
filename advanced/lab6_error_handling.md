---
layout: default
title: Lab 6 - Error Handling
---

# 🔹 Lab 6: Error Handling with Meraki SDK

## 🎯 Objective:
Add reliability to your automation scripts with exception handling.

```python
from meraki.exceptions import APIError

try:
    devices = dashboard.networks.getNetworkDevices("invalid_id")
except APIError as e:
    print(f"API failed: {e}")
```
