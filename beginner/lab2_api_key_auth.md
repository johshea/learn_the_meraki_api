---
layout: default
title: Lab 2 - API Key Authentication
---

# 🔹 Lab 2: Authenticating and Exploring the API

## 🎯 Objective:
Understand how to authenticate with the Meraki API and explore the available endpoints.

## 📘 Steps:

1. Go to the [Meraki Dashboard](https://dashboard.meraki.com)
2. Click on your profile > Generate API Key
3. Save it somewhere safe — it will not be shown again
4. Use it in headers in Postman or scripts:
   ```
   X-Cisco-Meraki-API-Key: <your_api_key>
   ```

## 🔗 Helpful Endpoints
- `/organizations`
- `/organizations/{orgId}/networks`
- `/networks/{networkId}/devices`
