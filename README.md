<div align="center">

# 📧 Smart Email Summarizer & Instant Alert System

<img src="https://img.shields.io/badge/Workflow-n8n_Automation-EA4B71?style=for-the-badge&logo=n8n&logoColor=white"/>
<img src="https://img.shields.io/badge/AI_Engine-Groq_LPU_Inference-F55036?style=for-the-badge&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/Notifications-Telegram_Bot_API-26A5E4?style=for-the-badge&logo=telegram&logoColor=white"/>
<img src="https://img.shields.io/badge/Protocol-IMAP_Integration-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
<img src="https://img.shields.io/badge/Type-Event_Driven_Automation-10B981?style=for-the-badge&logo=fastapi&logoColor=white"/>

<br/><br/>

> **An intelligent email automation workflow built with n8n. Listens for incoming emails via IMAP, leverages Groq AI for instant categorization and high-speed summarization, and dispatches real-time structured alerts directly to Telegram.**

</div>

---

## 📌 Executive Overview

Tired of overflowing inboxes and notification fatigue, this automation creates an intelligent triage layer between incoming emails and the user:

- **Automated Ingestion:** Listens to any IMAP-enabled email provider (Gmail, Outlook, custom domains) in real time.
- **Ultra-Fast LLM Processing:** Utilizes **Groq AI** (powered by high-speed LPUs) to analyze email headers, classify urgency, and extract concise action items.
- **Noise Reduction:** Automatically filters newsletters and spam, forwarding only critical, high-priority summaries.
- **Instant Messaging Delivery:** Sends structured markdown summaries directly to a private **Telegram** chat or channel.

---

## 📸 Workflow & Execution Previews

### 1. n8n Automation Workflow Graph
<p align="center">
  <img src="The%20Automation%20Workflow.jpeg" alt="n8n Workflow Graph" width="95%">
</p>

### 2. Telegram Alert Output
<p align="center">
  <img src="Telegram%20Notification.jpeg" alt="Telegram Notification Preview" width="60%">
</p>

---

## 🔄 Workflow Execution Lifecycle

```
[ Incoming Email ]
       │
       ▼ (IMAP Trigger)
[ n8n Email Node ] ──► Extract (Sender, Subject, Body)
                               │
                               ▼
                        [ Groq AI Node ]
                               │ (LLM Analysis & Triage)
                               ├── Classify: Important vs. Low Priority
                               └── Generate 3-bullet summary
                               │
                               ▼
                     [ Filter / IF Node ]
                               │ (Pass only "Important")
                               ▼
                     [ Telegram Bot Node ]
                               │
                               ▼ (Markdown Message)
                     [ User's Phone / Desktop ]
```

---

## 🛠️ Tech Stack & Integrations

| Component | Service / Technology | Purpose |
|---|---|---|
| **Orchestration** | **n8n** (Self-hosted or Cloud) | Visual workflow orchestration and event scheduling |
| **AI Inference** | **Groq AI API** (Llama 3 / Mixtral) | Sub-second email classification and concise summary extraction |
| **Notification Channel** | **Telegram Bot API** | Real-time push alert delivery with formatted markdown |
| **Mail Protocol** | **IMAP / SSL** | Universal secure inbox polling and message extraction |

---

## ⚙️ Quick Setup Guide

1. **Import Workflow:**
   - In your n8n canvas, select **Import from File** and choose `workflow.json`.
2. **Configure Credentials:**
   - **IMAP Account:** Enter your email address and app-specific password with SSL enabled.
   - **Groq API Key:** Add your Groq API credentials.
   - **Telegram Bot:** Add your Telegram Bot Token and destination `chat_id`.
3. **Activate & Test:**
   - Turn the workflow toggle to **Active**.
   - Send a test email to your inbox to observe the instant Telegram alert.

---

## 📬 Author & Connect

<div align="center">

**Developed by Rafat Ashraf**  
*Cloud & DevOps Engineer*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/rafat-devops)

</div>
