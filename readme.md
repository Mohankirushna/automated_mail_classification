# 📬 Intelligent Gmail Automation using n8n 🚀

Welcome to an exciting automation project that streamlines your email management using [n8n](https://n8n.io/)! This repository contains **two versions** of a smart email classification and notification system:

---

## 🧠 Version 1: `full_working_workflow_6` (Gemini + Telegram Bot Integration)
![Workflow Preview](https://github.com/user-attachments/assets/f41255e1-0584-43ee-ace1-d3cf29a53cbc)

### ✨ What it does:

✅ Automatically triggers when a **new email** arrives in your Gmail inbox  
🧠 Sends the email content (subject + body) to **Gemini 1.5 Flash API** for classification  
🏷️ Gemini classifies it into one of the following labels:
- `college`
- `internship`
- `placement`
- `finance`
- `events`
- `other`

📌 The email is then **moved into the appropriate Gmail label** automatically  
📢 A notification is sent to your personal **Telegram chatbot** (named `Marko`) with:
- ✅ Classified label
- 📨 Email subject
- 🧾 Message ID

---

### ⚙️ Tools Used

- 🔗 [n8n](https://n8n.io/) (Open-source workflow automation)
- 💌 Gmail API (for email access and label manipulation)
- 🔮 Gemini 1.5 Flash API (for AI-powered email classification)
- 🤖 Telegram Bot API (to notify you in real-time via chat)
- 🌐 Ngrok (for local webhook tunneling)

---

## 🧩 Version 2: `My_workflow_6` (Minimal Email Sorter)
![Workflow Preview](![image](https://github.com/user-attachments/assets/c935f088-2c85-4dfd-9099-8a174352ec43)


### ✨ What it does:

✅ Automatically triggers when a **new email** arrives in your Gmail inbox  
🏷️ Applies simple, rule-based logic (via `Switch` nodes) to classify the email into categories such as:
- `college`
- `internship`
- `placement`
- `finance`
- `events`
- `other`

📌 Emails are directly moved to their respective Gmail labels without any AI-based classification  
❌ No Gemini integration  
❌ No Telegram notifications

---

### ⚙️ Tools Used

- 🔗 [n8n](https://n8n.io/)
- 💌 Gmail API

This version is lightweight, fast, and suitable for simple rule-based email management setups.

---

