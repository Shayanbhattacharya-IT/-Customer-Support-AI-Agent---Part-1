# 🤖 Customer Support AI Agent - Part 1

An AI-powered Customer Support Assistant built using **n8n**, **Google Gemini**, **Telegram Bot**, and **Google Sheets**.

This project demonstrates how businesses can automate customer support by allowing users to interact with an AI assistant through Telegram. The bot searches a Knowledge Base stored in Google Sheets, generates intelligent responses using Google Gemini, and provides a seamless support experience.

> 🚀 This is **Part 1** of the project. Future versions will include Jira ticket creation, ticket tracking, and real-time notifications.

---

# 📌 Project Overview

The Customer Support AI Agent helps users get answers to common IT or business-related questions without requiring human intervention.

If the AI cannot answer a question, future versions of this project will automatically create a Jira ticket and notify both the support team and the user.

This project was built using a **No-Code/Low-Code Automation** approach with n8n.

---

# 🎯 Objectives

- Automate customer support
- Reduce repetitive support requests
- Provide instant AI-generated responses
- Use Google Sheets as a simple Knowledge Base
- Demonstrate AI workflow automation using n8n

---

# 🛠 Tech Stack

| Technology | Purpose |
|------------|---------|
| n8n | Workflow Automation |
| Google Gemini AI | AI Response Generation |
| Telegram Bot | User Interface |
| Google Sheets | Knowledge Base |
| Telegram Bot API | Communication |

---

# 🏗 Architecture

```
                User
                  │
                  │
          Telegram Bot
                  │
                  ▼
           n8n Workflow
                  │
     ┌────────────┴────────────┐
     │                         │
     ▼                         ▼
Google Sheets            Google Gemini AI
(Knowledge Base)        (Generate Response)
     │                         │
     └────────────┬────────────┘
                  │
                  ▼
         AI Response Returned
                  │
                  ▼
           Telegram User
```

---

# 🚀 Features (Current Version)

✅ Telegram Bot Interface

✅ AI-powered Question Answering

✅ Google Sheets Knowledge Base

✅ Google Gemini Integration

✅ No-Code Automation

✅ Interactive Telegram Menu

---

# 📂 Project Workflow

```
Telegram User

      │

      ▼

Telegram Bot

      │

      ▼

n8n Workflow Trigger

      │

      ▼

Receive User Question

      │

      ▼

Read Knowledge Base
(Google Sheets)

      │

      ▼

Send Context
to Google Gemini

      │

      ▼

Generate AI Response

      │

      ▼

Return Response
to Telegram User
```

---

# 📑 Workflow Explanation

### Step 1

User opens the Telegram Bot.

---

### Step 2

The bot displays the welcome menu.

```
🤖 Welcome to TechAssist AI

🔍 Ask IT Question

🎫 Create Ticket (Coming Soon)

📋 My Tickets (Coming Soon)

ℹ️ Help
```

---

### Step 3

The user selects **Ask IT Question**.

---

### Step 4

The user enters a question.

Example:

```
How do I reset my VPN password?
```

---

### Step 5

n8n reads the Knowledge Base from Google Sheets.

---

### Step 6

The relevant information is sent to Google Gemini.

Prompt Example:

```
You are an IT Support Assistant.

Use the following Knowledge Base to answer.

<context from Google Sheets>

User Question:
How do I reset my VPN password?
```

---

### Step 7

Google Gemini generates the best possible response.

---

### Step 8

The response is returned to Telegram.

Example:

```
To reset your VPN password:

1. Open VPN Portal
2. Click Forgot Password
3. Verify your email
4. Create a new password

If the issue persists, contact IT Support.
```

---

# 📊 Google Sheets Structure

Example Knowledge Base

| Category | Question | Answer |
|----------|----------|--------|
| VPN | Reset VPN Password | Open VPN Portal → Forgot Password |
| Outlook | Outlook Not Opening | Restart Outlook and Clear Cache |
| Printer | Printer Offline | Restart Printer Service |
| Laptop | Slow Laptop | Restart Device and Clear Temporary Files |

---

# 📸 Screenshots

Add screenshots here.

Example:

```
/screenshots

telegram-home.png

telegram-chat.png

google-sheet.png

n8n-workflow.png
```

---

# 📂 Folder Structure

```
Customer-Support-AI-Agent/

│

├── README.md

├── screenshots/

├── workflow/

│      CustomerSupport.json

├── docs/

│      Architecture.png

│      Workflow.png

└── assets/
```

---

# ⚙ Setup Guide

## 1. Clone Repository

```bash
git clone https://github.com/yourusername/customer-support-ai-agent.git
```

---

## 2. Create Telegram Bot

Create a bot using BotFather.

Copy the Bot Token.

---

## 3. Create Google Sheet

Create columns:

- Category
- Question
- Answer

Share the sheet with your Google Service Account.

---

## 4. Create Google Gemini API Key

Generate an API Key from Google AI Studio.

---

## 5. Configure n8n

Add credentials for:

- Telegram
- Google Sheets
- Google Gemini

---

## 6. Import Workflow

Import the provided n8n workflow JSON.

Activate the workflow.

---

# 📈 Future Roadmap (Part 2)

The next version will include:

- ✅ Jira Ticket Creation
- ✅ Ticket Status Updates
- ✅ Ticket Assignment
- ✅ Real-time Telegram Notifications
- ✅ Escalation Workflow
- ✅ Conversation Memory
- ✅ Multi-user Support
- ✅ AI Confidence Score
- ✅ Human Handoff
- ✅ Analytics Dashboard

---

# 💡 Possible Improvements

- Vector Database
- Pinecone Integration
- Supabase
- LangChain
- RAG Architecture
- OpenAI Support
- Claude Support
- Multi-language Support

---

# 🎥 Demo

Coming Soon

---

# 📺 YouTube

Watch the complete project walkthrough here:

> Add your YouTube Link

---

# 📄 Documentation

The repository contains:

- Architecture Diagram
- Workflow Documentation
- Screenshots
- n8n Workflow
- Setup Guide

---

# 🤝 Contributing

Contributions are welcome!

If you'd like to improve this project, feel free to:

- Fork the repository
- Create a new branch
- Submit a Pull Request

---

# ⭐ Support

If you found this project useful, please consider giving it a ⭐ on GitHub.

It helps others discover the project and motivates future development.

---

# 📬 Contact

**Shayan Bhattacharya**

LinkedIn:
(Add your LinkedIn URL)

GitHub:
(Add your GitHub URL)

Email:
(Add your Email)

---

# 📜 License

This project is licensed under the MIT License.

---

## 🚀 Part 2 Coming Soon

Upcoming features include:

- Jira Integration
- AI Ticket Routing
- Ticket Notifications
- Approval Workflow
- Advanced AI Agent
- Enterprise Customer Support Automation
