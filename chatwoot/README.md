[<- Back](/)

# ChatWoot WhatsApp Integration
<p align="center">
    <img 
        src="./waha-chatwoot.png"
        height=300
    />
</p>

You can integrate 
[WAHA](https://waha.devlike.pro)
with
[ChatWoot](https://www.chatwoot.com/)
to receive and send messages to WhatsApp via n8n.

# How it works
We'll guide you through the setup steps for each template.

## 1. Database Migration
[**template.json**](./WhatsApp___ChatWoot__Database_Migrations.json)

1. Import [template.json](./WhatsApp___ChatWoot__Database_Migrations.json) to **n8n**
2. Configure **Posgres** nodes with your Postgres credentials
3. Run **Migration** block to create the necessary tables

## 2. WAHA => ChatWoot

[**template.json**](./WhatsApp___ChatWoot__WAHA____ChatWoot_Messages.json)

The workflow **receives** messages from WhatsApp via WAHA and sends them to ChatWoot.
1. Go to **ChatWoot** and create new **Inbox**
2. Get from the **Inbox** settings and **ChatWoot** settings:
   1. **Account ID**
   2. **Inbox ID**
   3. **Inbox Identifier**
   4. **ChatWoot URL**
3. Import [template.json](./WhatsApp___ChatWoot__WAHA____ChatWoot_Messages.json) to **n8n**
4. Set settings from **ChatWoot** in the workflow
5. Set all **Postgres** nodes with your Postgres credentials
6. Set all **ChatWoot** nodes with your **ChatWoot** credentials
7. **Active** your workflow in n8n
8. Copy **URL** from **Webhook** node
9. Paste it in your **WAHA** session webhook settings and configure to listen `message` events
10. Send a test message from WhatsApp to see it in ChatWoot




