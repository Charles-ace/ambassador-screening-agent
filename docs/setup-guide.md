# Setup Guide — Ambassador Screening Agent

This guide explains how to install and run the Ambassador Screening Agent in under 15 minutes.

---

# 1. Requirements

Before starting, make sure you have:

* n8n account (cloud or self-hosted)
* Google account (for Sheets + Forms)
* OpenAI API key
* Telegram bot (created via BotFather)

---

# 2. Import the Workflow

1. Open n8n
2. Go to **Workflows**
3. Click **Import Workflow**
4. Upload:

```
workflow/ambassador-screening-agent.json
```

5. Click **Save**

---

# 3. Setup Google Sheets

Create a Google Sheet with these columns:

```
Timestamp
Name
Email
X handle
Experience Level
Motivation
Signal Score
Status
AI Score
AI Reason
```

Then:

* Copy Sheet ID from URL
* Connect Google Sheets credential in n8n
* Select the correct sheet tab

---

# 4. Connect OpenAI

In n8n:

* Go to Credentials
* Add OpenAI API Key
* Attach it to LLM node

---

# 5. Setup Telegram Bot

1. Create bot via @BotFather
2. Get Bot Token
3. Add bot to Telegram group
4. Make bot admin
5. Copy Chat ID
6. Paste into Telegram node in n8n

---

# 6. Activate Workflow

Once everything is connected:

* Click **Activate Workflow**
* Submit a test form entry
* Check:

  * Google Sheets updates
  * AI score generated
  * Telegram message sent

---

# How It Works

```
Google Form → Google Sheets → n8n Trigger
→ AI Evaluation (OpenAI)
→ Decision Engine (Code + IF nodes)
→ Google Sheets Update
→ Telegram Notification
```

---

# Troubleshooting

### No Telegram message

* Check bot is admin
* Check chat ID is correct

### No AI response

* Check OpenAI API key
* Check node connection

### Sheet not updating

* Check column names match exactly
* Check Email field exists

---

# Done

Your system is now live.
