# n8n-slack-daily-motivation-bot

A simple Slack bot built with **n8n** that sends **motivational quotes 3 times a day** using the [ZenQuotes API](https://zenquotes.io/).  
✅ Easy to use  
✅ Clean JSON  
✅ Perfect for productivity and positive vibes 🌞

---

## 💡 What it does

Ping (the bot) posts a motivational quote to Slack at:

- 🕗 08:00 – Morning Boost  
- 🕐 13:00 – Midday Reminder  
- 🕕 18:00 – Evening Motivation

---

## ⚙️ Requirements

- n8n (self-hosted or cloud)
- Slack account
- Slack App (with Bot Token or OAuth)
- ZenQuotes API (no API key required)

---

## 🚀 How to use

### 1. Download the JSON file  
Grab the workflow file:  
`n8n_slack_daily_motivation_bot_v140525.json`

### 2. Import into n8n  
- Go to `Workflows` → `Import from file`
- Upload the JSON file  
- Hit **Activate** when you’re ready

### 3. Create your Slack App  
- Visit [Slack API](https://api.slack.com/apps) and create a new app  
- Under **OAuth & Permissions**, add these scopes:
  - `chat:write`
  - `chat:write.public`
  - `channels:read`
- Install the app to your Slack workspace

### 4. Connect Slack to n8n  
Use either of these methods:
- **Bot Token**: easiest method, copy your `xoxb-...` token and paste it into n8n as Slack API credentials
- **OAuth2**: only if you want full OAuth flow (requires HTTPS and domain)

### 5. Set your Slack channel  
Make sure the bot is added to your channel.  
In the **Send to Slack** node:
- Select `Send Message To: Channel`
- Choose your channel (from list or by ID)

---

## 🖼️ Screenshots

### Workflow in n8n
![Workflow](https://raw.githubusercontent.com/TuguiDragos/n8n-slack-daily-motivation-bot/refs/heads/main/Worflow.png)

### Mobile Notification
![Notification](https://raw.githubusercontent.com/TuguiDragos/n8n-slack-daily-motivation-bot/main/Pingshot1.png)

---

## 📄 License

MIT - free to use, remix, and share good energy ⚡

---

Made with ☕ and n8n by [TuguiDragos.com](https://tuguidragos.com)
