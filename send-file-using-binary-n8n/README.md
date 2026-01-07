[<- Back](/)

# Send File using Binary N8N

[**template.json**](./template.json)

## How it works
This workflow downloads an image from a URL and sends it to WhatsApp using WAHA (WhatsApp HTTP API).
It demonstrates how to handle binary data in n8n and send it via `multipart/form-data` to WAHA.

## Set up steps
1. **Copy** template and **Paste** in n8n (Ctrl+V), or **Import From URL**.
2. Update the **Variables for Connect Waha API** node with your specific details:
   - `waha-api`: Your WAHA API endpoint for sending files (e.g., `http://your-waha-instance/api/sendFile`).
   - `chatId`: The WhatsApp chat ID where the file will be sent (e.g., `123456789@c.us` or `123456789@g.us`).
   - `session`: Your WAHA session name (e.g., `default`).
   - `X-Api-Key`: Your WAHA API Key (if authentication is enabled).
3. (Optional) In the **get images** node, you can change the URL to download a different image or file.
4. Execute the workflow.

The workflow will:
1. Fetch the image from the specified URL.
2. Send the image to the specified WhatsApp chat via your WAHA instance.
