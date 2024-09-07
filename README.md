# WAHA n8n Templates Gallery

<p align="center">
  <img src="./WAHA+n8n.png" width='300'/>
</p>

Templates for [WAHA - WhatsApp HTTP API](https://waha.devlike.pro) and [n8n](https://n8n.io/) workflows using
[@devlikeapro/n8n-nodes-waha](https://github.com/devlikeapro/n8n-nodes-waha) 
node.
- [WAHA](https://waha.devlike.pro) - **WhatsApp API** that you can run in a click!
- [@devlikeapro/n8n-nodes-waha](https://github.com/devlikeapro/n8n-nodes-waha) 
- [n8n](https://n8n.io/) is a [fair-code licensed](https://docs.n8n.io/reference/license/) workflow automation platform.


# How to use the templates

You can import the workflows:
1. Go to your n8n installation with installed **WAHA** node.
2. **Add workflow** there (just empty one)
3. Import one of the **templates** by clicking on three dots **...** at the right top corner
	 of the n8n window and selecting **Import from URL**.
4. Paste the url to import workflow
5. Select credentials for all WAHA nodes
6. Configure you session to send event to **WAHA Trigger** Webhook URL
7. Activate the workflow
8. Enjoy low-code automation!


# Workflows Templates
![](chatting-template/workflow.png)

👉 Checkout folders for more templates!

- [Chatting Template](./chatting-template) - Simple chatting template that replies with "pong" if received "ping" and sends an image if received "image".
- [Send QR code to Email](./send-qr-code-to-email) - Send QR code to the email when session it's in `SCAN_QR_CODE` status.
- [Forward all text messages to email](./forward-all-text-messages-to-email)
- [Send Custom HTTP Request to WAHA API](./send-custom-http-request-to-waha)
- [Restart server at midnight](./restart-server-at-midnight)
- [WAHA Trigger Explanation](./waha-trigger-explanation)
