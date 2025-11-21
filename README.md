
# 🤖 Automated ATS Resume Screening Telegram Bot using n8n

## 📌 Project Overview
This project automates ATS (Applicant Tracking System) resume screening using **n8n** and **Telegram Bot**. 
Users can upload **PDF** or **ZIP** files through Telegram, and the system extracts candidate details, evaluates resumes with AI, generates an **ATS Score**, and stores results in **Google Sheets**. It also sends automated emails to accepted/rejected candidates.

---

## 🚀 Features
- Real-time resume scanning through Telegram chat
- Accepts **single PDF** or **ZIP with multiple resumes**
- AI-based ATS score generation (1–100)
- Automatically extracts **Name, Email, Mobile Number**
- Saves shortlisted candidates to **Google Sheets**
- Sends **acceptance & rejection emails** automatically via Gmail
- Loop processing for bulk ZIP resumes

---

## 🧠 Tech Stack
| Component | Technology |
|-----------|-----------|
| Automation | n8n |
| Messaging | Telegram Bot API |
| AI Model | Gemini / LangChain Agent |
| Storage | Google Sheets |
| File Extraction | PDF & ZIP processing |
| Email | Gmail Automation |

---

## 📂 Project Workflow
1. User sends **“Hi/Hello/Hey”** in Telegram → bot responds asking to upload resume
2. User uploads **PDF / ZIP**
3. ZIP resumes are looped and processed sequentially
4. AI calculates ATS Score and extracts candidate data in JSON
5. If score > 70 → stored in **Accepted Sheet** & **Acceptance email sent**
6. Else → stored in **Rejected Sheet** & **Rejection email sent**
7. Bot sends final status response


