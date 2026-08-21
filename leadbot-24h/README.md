# LeadBot 24h — AI WhatsApp Lead Qualification Bot

[**template.json**](./template.json)

AI-powered n8n workflow that captures WhatsApp messages, scores lead intent with free AI (Google Gemini), and routes hot prospects to sales — 24/7, zero monthly API cost.

## What it does

| Step | Action |
|------|--------|
| 1 | Receives incoming WhatsApp message via webhook |
| 2 | AI scores lead intent from 1 to 5 (free Gemini tier) |
| 3 | Score ≥ 3 → instant WhatsApp alert to sales |
| 4 | Score < 3 → silently archived |
| 5 | Every lead gets auto-reply: "received, we'll get back in 10 minutes" |

## Set up

1. **Import** `template.json` into n8n (File → Import or Ctrl+V)
2. **Configure** webhook URL and point your WhatsApp sender (WAHA or any HTTP trigger) to it
3. **Activate** the workflow
4. Done — no paid APIs, no monthly costs

## Requirements

- n8n instance (cloud or self-hosted)
- Free Google Gemini API key ([get one here](https://aistudio.google.com/apikey))
- Any WhatsApp HTTP API (WAHA, Twilio, or custom webhook)

## Full version

This is the **Lite edition** (2 nodes, core lead capture + scoring).  
Full version with advanced qualification logic, CRM routing, and Google Sheets sync:  
👉 https://planificador7.gumroad.com/l/leadbot-24h?utm_source=github&utm_medium=free_template&utm_campaign=leadbot24h&utm_content=devlikeapro-waha
