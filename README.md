# 🤖 n8n AI Email Agent

An AI-powered email automation agent built with **n8n** that understands natural-language email requests, identifies the intended recipients from an Excel contact database, generates a professional email, and sends it through Gmail.

## 🚀 Features

- 💬 Natural-language email requests
- 🤖 AI-powered recipient and email generation
- 📊 Excel-based contact management
- 👤 Send emails to a person or list
- 🔢 Send emails to a specific ID range
- 🏢 Filter recipients by department/role
- 👥 Filter recipients by group/category
- 📧 Gmail integration
- 🛡️ Maximum recipient safety limit
- 🚫 Filters placeholder email addresses

## 🧠 How It Works

```text
User Request
     ↓
n8n Chat Trigger
     ↓
AI Agent
     ↓
Read Excel Contacts
     ↓
Filter Recipients
     ↓
Attach Generated Email
     ↓
Gmail
     ↓
Send Email
```

The AI Agent interprets the user's request and determines the target type, target value, email subject, and email body.

The workflow then reads the contact database, filters the matching recipients, applies a safety limit, and sends the generated email through Gmail.

## 🛠️ Tech Stack

- **n8n** — Workflow automation
- **AI Agent** — Natural-language request processing
- **Groq** — LLM provider
- **GPT-OSS-20B** — Language model
- **Gmail** — Email delivery
- **Excel (XLSX)** — Contact database
- **JavaScript** — Recipient filtering and processing

## 💬 Example Requests

```text
Send an email to Priya Verma about the internship opportunity.

Send an email to the first 10 contacts.

Send an email to everyone in HR.

Send an email to the Internship group.
```

## ⚙️ Setup

1. Import `workflow.json` into n8n.
2. Configure your own Gmail OAuth2 credentials.
3. Configure your own Groq API credentials.
4. Create your own contacts Excel file.
5. Update the Excel file path in the workflow.
6. Run the workflow.

> **Note:** `sample_contacts.xlsx` is included as a demonstration contact database. Replace it with your own contact file when running the workflow.

## 🔐 Security

This repository does not contain:

- API keys
- OAuth tokens
- Client secrets
- Passwords
- Personal contact information
- Private credentials

Users must configure their own credentials before running the workflow.

## 📁 Project Structure

```text
n8n-ai-email-agent/
│
├── workflow.json
├── sample_contacts.xlsx
├── workflow.png
└── README.md
```

## 🔮 Future Improvements

- Email scheduling
- Email templates
- Follow-up automation
- Delivery tracking
- Email analytics
- Improved contact management
