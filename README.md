# 📧🤖 AI Email-to-Calendar Assistant with n8n

## 📌 Overview
This project is an **automation workflow built with n8n** that connects **Gmail**, an **AI Agent**, and **Google Calendar**.  

The assistant can:  
- Watch incoming Gmail messages.  
- Interpret the email content using an AI model.  
- Automatically create or update Google Calendar events.  
- Reply back with a confirmation.  

This setup turns your inbox into a **smart scheduling assistant**.  

---

## 🛠️ Tech Stack
- [n8n](https://n8n.io/) – automation platform  
- Gmail 
- AI Agent 
- Google Calendar 

---

## ⚙️ Workflow Design

### 1. **Trigger**
- Workflow starts with a **Gmail Trigger** node when a new email arrives.  

### 2. **AI Agent**
- The email content is passed to an **AI Agent Node**.  
- The model determines intent:
  - *Is this an event request?*  
  - *Does it provide start/end times, title, description?*  

### 3. **Google Calendar Integration**
- **Create Event** – if the AI extracts valid details.  
- **Get Many Events** – to check if the time slot is free.  


---

## Workflow Example
<img width="1073" height="497" alt="image" src="https://github.com/user-attachments/assets/7f7e2f42-9259-44d6-a467-f9f4f61c7bb4" />


### Example 1: Read Events
**User:**  
