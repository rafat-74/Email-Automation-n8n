# 📧 Smart Email Summarizer

An intelligent automation system built with **n8n** that helps you stay on top of your inbox without the clutter. It filters incoming emails, summarizes the important ones using **Groq AI**, and notifies you instantly via **Telegram**.

## 🚀 How It Works
1. **Trigger:** Automatically listens for new incoming emails via IMAP.
2. **AI Processing:** Groq AI analyzes the email content to filter out spam and summarize essential details.
3. **Smart Notification:** Only "Important" updates are forwarded to your Telegram bot.

## 🛠️ Tech Stack
- **n8n:** The orchestration engine.
- **Groq AI:** Used for intelligent text summarization.
- **Telegram Bot API:** For real-time notifications.
- **IMAP:** To connect and monitor email accounts.

### 📸 Workflow & Result

**The Automation Workflow:**
![Workflow](The%20Automation%20Workflow.jpeg)

**Telegram Notification:**
![Telegram](Telegram%20Notification.jpeg)

## ⚙️ How to Setup
1. Import the `workflow.json` file into your n8n instance.
2. Configure your IMAP credentials.
3. Add your Telegram Bot Token and your Chat ID.
4. Set up your Groq AI API key.
5. Activate the workflow and enjoy!

---
*Built with ❤️ by [Your Name]*
