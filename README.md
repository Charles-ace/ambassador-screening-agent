# Ambassador Screening Agent

AI-powered ambassador application screening system built with **n8n**, **OpenAI**, **Google Sheets**, and **Telegram**.
It automatically evaluates applicants, assigns scores, and sends structured decisions to campaign managers in real time.

---

## What this project does

The Ambassador Screening Agent automates the entire ambassador application review process:

* Collects applications from Google Forms / Google Sheets
* Uses AI to evaluate candidates based on experience and signals
* Assigns a structured score (0–100)
* Classifies applicants into:

  * **Accepted**
  * **Review**
  * **Rejected**
* Updates Google Sheets automatically
* Sends real-time reports to Telegram for campaign managers

---

## How it works

```text
Google Form → Google Sheets → n8n Trigger → AI Evaluation (OpenAI)
→ Code Processing → Decision Routing → Google Sheets Update → Telegram Notification
```

---

## Tech Stack

* n8n (automation engine)
* OpenAI (LLM scoring & reasoning)
* Google Sheets (database)
* Telegram Bot (manager notifications)

---

## Decision Logic

* **70–100** → Accepted
* **40–69** → Review
* **0–39** → Rejected

Each decision includes:

* AI-generated score
* Reasoning explanation
* Structured classification

---

## 📦 Features

* Fully automated applicant screening
* AI-powered scoring system
* Real-time Telegram notifications
* Google Sheets as lightweight CRM
* Easy plug-and-play deployment
* No-code / low-code setup

---

## 🛠️ Setup Instructions

1. Import the n8n workflow JSON
2. Connect credentials:

   * Google Sheets API
   * OpenAI API Key
   * Telegram Bot Token
3. Create a Google Sheet using the provided template
4. Connect Google Form (optional)
5. Activate workflow

---

## Project Structure

```
ambassador-screening-agent/
│
├── workflow/               # n8n workflow JSON
├── templates/              # Google Sheet + form templates
├── docs/                   # setup & architecture guides
├── screenshots/           # UI & workflow images
└── README.md
```

---

## Use Cases

* Web3 ambassador programs
* DAO contributor onboarding
* Startup community management
* Hackathon application screening
* Growth & marketing campaigns

---

## Why this matters

Manual ambassador screening is slow, inconsistent, and hard to scale.

This system:

* Reduces manual review time
* Standardizes decision-making
* Provides transparent scoring
* Enables real-time campaign visibility

---

## Future Improvements

* Email notifications for applicants
* Daily digest reports for managers
* Advanced scoring models
* Multi-campaign support
* Dashboard UI layer

---

## Author

Built as a portfolio project demonstrating AI automation, workflow design, and real-world product thinking.

---

## 📜 License

MIT (or choose your preferred license)
