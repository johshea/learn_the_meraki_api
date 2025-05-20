---
layout: default
title: Lab 4 - Intro to Meraki Python SDK
---

# 🔹 Lab 4: Intro to Meraki SDK

## 🎯 Objective:
Use Cisco's official Python SDK to authenticate and fetch basic org/network data.

## 🔧 Installation:
```bash
pip install meraki
```

## 🧪 Sample Code:
```python
import meraki

dashboard = meraki.DashboardAPI(api_key='your_api_key')
orgs = dashboard.organizations.getOrganizations()

for org in orgs:
    print(f"{org['name']} - {org['id']}")
```
