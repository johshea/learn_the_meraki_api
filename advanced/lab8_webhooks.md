---
layout: default
title: Lab 8 - Webhooks
---

# 🔹 Lab 8: Webhook Receiver

## 🎯 Objective:
Listen for real-time alerts from Meraki

```python
from flask import Flask, request
app = Flask(__name__)

@app.route('/webhook', methods=['POST'])
def webhook():
    print(request.json)
    return '', 200

app.run(port=5001)
```

Then register your webhook URL in the Meraki dashboard under Organization > Settings > Webhooks.
