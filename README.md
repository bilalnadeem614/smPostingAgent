# smPostingAgent

# 🤖 Social Auto-Poster Agent (n8n + Gemini)

An AI-powered Telegram bot that auto-posts content from Google Drive to **Twitter (X), LinkedIn, YouTube, and Telegram Group** — all triggered by a simple `/post` command.

[Demo] https://youtu.be/SrJLgTsKd8A 

---

## ✨ Features
- 📩 **Trigger via Telegram**: Send `/post` in private chat
- 📁 **Fetch from Google Drive**: Pulls text, image, and video from a "Content" folder
- 🧠 **AI Optimization**: Uses **Gemini** to tailor content per platform:
  - **Twitter**: ≤280 characters
  - **LinkedIn**: Professional tone, ≤3,000 chars
  - **YouTube**: Title + description generation
  - **Telegram Group**: Full text + media
- 🔒 **Secure**: Only responds to private commands (ignores groups)
- ⚙️ **Self-Hosted**: Runs on your machine (via ngrok)

---

## 🛠️ Tech Stack
- **Automation**: [n8n v1.117.3](https://n8n.io/)
- **AI**: Google Gemini (`gemini-pro`)
- **Messaging**: Telegram Bot API
- **Storage**: Google Drive
- **Tunnel**: ngrok (for local dev)


## 🚀 Setup Guide

### Prerequisites
1. [n8n](https://docs.n8n.io/hosting/installation/) installed locally
2. [ngrok](https://ngrok.com/) account
3. API credentials for:
   - Telegram Bot
   - Google Drive
   - Twitter (X) Developer Account
   - LinkedIn Developer App
   - YouTube Data API v3
