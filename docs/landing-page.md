# Ambassador Screening Agent

AI-powered system that automatically screens, scores, and ranks ambassador applications in real time.

---

# The Problem

Most Web3 and startup ambassador programs face the same issue:

* Too many applicants
* Manual screening is slow
* Decisions are inconsistent
* Good candidates get missed

---

# The Solution

The Ambassador Screening Agent automates the entire process:

* Collect applications via Google Forms
* Use AI to evaluate each applicant
* Assign a structured score (0–100)
* Classify applicants into:

  * Accepted
  * Review
  * Rejected
* Notify campaign managers instantly on Telegram
* Store everything in Google Sheets

---

# How It Works

```text id="flow1"
Google Form → Google Sheets → n8n Trigger
→ OpenAI Evaluation
→ Scoring Engine
→ Decision Routing
→ Google Sheets Update
→ Telegram Notification
```

---

# Decision Logic

* 70–100 → Accepted (strong candidates)
* 40–69 → Review (manual check needed)
* 0–39 → Rejected (not a fit)

---

# Who This Is For

* Web3 DAO ambassador programs
* Startup growth teams
* Community managers
* Hackathon organizers
* Marketing teams handling applications

---

# Features

* Fully automated applicant screening
* AI-powered scoring and reasoning
* Real-time Telegram alerts
* Google Sheets as lightweight CRM
* No-code deployment via n8n
* Plug-and-play setup (15 minutes)

---

# Why It Matters

Instead of manually reviewing applications:

👉 You get instant structured decisions
👉 You reduce screening time by 90%+
👉 You standardize evaluation across all applicants

---

# What You Get

* n8n workflow JSON
* Setup guide
* Google Sheet template
* Telegram integration
* Fully working automation system

---

# Setup Time

⏱ ~10–15 minutes

No coding required.

---

# Get Started

1. Import workflow into n8n
2. Connect OpenAI + Google Sheets + Telegram
3. Activate workflow
4. Start screening applicants automatically

---

# Built for scale

Designed to handle:

* small communities
* large DAO programs
* high-volume applications
