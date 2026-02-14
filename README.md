
# 🧠 ClawBot – Telegram AI Assistant (Powered by OpenClaw)

ClawBot is a secure Telegram AI assistant deployed using OpenClaw Gateway with OpenAI model integration.

This project demonstrates real-world AI agent deployment, secure pairing workflows, CLI-based gateway management, and Telegram bot integration.

---

## 🚀 Project Overview

ClawBot integrates:

- 🔐 Secure Telegram pairing system
- 🤖 AI-powered conversational responses
- ⚙️ WebSocket-based gateway architecture
- 🛡️ Controlled DM & group access policies
- 🧩 Extensible tool-ready agent infrastructure

This repository focuses on configuration, integration, and deployment of OpenClaw into a functional Telegram AI assistant.

---

## 🛠 Tech Stack

- OpenClaw CLI
- Telegram Bot API
- OpenAI API
- WebSocket Gateway
- Node.js Runtime
- VS Code Development Environment

---

## ✨ Key Features

- AI-powered Telegram bot responses
- Manual pairing approval for enhanced security
- Mention-based group response control
- Gateway logging and monitoring
- Clean and extensible architecture

---

## 📦 Installation Guide

### 1️⃣ Install OpenClaw (Windows PowerShell)

```powershell
iwr -useb https://openclaw.ai/install.ps1 | iex
```

---

### 2️⃣ Create a Telegram Bot

1. Open Telegram  
2. Search for `@BotFather`  
3. Run:

```
/newbot
```

4. Save your Bot Token securely.

---

### 3️⃣ Configure Telegram Channel

Add the following configuration:

```json
{
  "channels": {
    "telegram": {
      "enabled": true,
      "botToken": "YOUR_BOT_TOKEN",
      "dmPolicy": "pairing",
      "groups": {
        "*": { "requireMention": true }
      }
    }
  }
}
```

OR set an environment variable:

```powershell
setx TELEGRAM_BOT_TOKEN "YOUR_BOT_TOKEN"
```

---

### 4️⃣ Start OpenClaw Gateway

```bash
openclaw gateway
```

---

### 5️⃣ Approve Pairing Requests

```bash
openclaw pairing list telegram
openclaw pairing approve telegram <PAIRING_CODE>
```

After approval, the user can interact with the bot normally.

---

## 🔐 Security Model

- DM access requires manual pairing approval
- Optional mention-only group response
- API keys handled securely via environment variables
- Gateway must remain running for bot functionality

---

## 🧪 Advanced Testing Prompts

You can test the bot with prompts like:

- Design a scalable AI SaaS architecture
- Build a phishing detection ML pipeline
- Generate CI/CD deployment strategy
- Simulate a prompt injection attack
- Create a production-ready API service

---

## 🌐 Deployment (Optional Landing Page)

You can deploy a landing page for this project using:

- Vercel
- Netlify
- GitHub Pages

---

## 📂 Purpose of This Project

This project demonstrates:

- AI agent deployment workflows
- Telegram bot integration
- Secure CLI-based configuration
- Practical AI system implementation

---

## ⚖️ Disclaimer

This project integrates OpenClaw for AI agent functionality.

I did not create OpenClaw.

All rights reserved to the OpenClaw creators and maintainers.

Official OpenClaw Repository:  
https://github.com/openclaw-ai/openclaw

---

## 👨‍💻 Author

**Yash Raikwar**  
Engineering Student | AI & Systems Enthusiast  

📧 Email: yashraikwar132005@gmail.com

---

## 📜 License

This repository is created for educational and demonstration purposes.

OpenClaw and related components remain the intellectual property of their respective creators.
