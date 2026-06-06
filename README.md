# n8n-workflows:
# AI Automation – Scheduled Email Workflow

A beginner-friendly AI automation project built with **n8n** (self-hosted), demonstrating how to send automated scheduled emails without writing any code.

---

## What This Workflow Does

Automatically sends an email to a specified recipient on a fixed schedule using Gmail SMTP.

---

## Workflow Overview

```
Schedule Trigger → Send an Email
```

| Node | Role |
|------|------|
| Schedule Trigger | Fires the workflow at a set time/interval |
| Send an Email | Sends email via Gmail SMTP to the recipient |

---

## Tools Used

- [n8n](https://n8n.io) – Self-hosted workflow automation
- Gmail SMTP – Email delivery
- Node.js – Required to run n8n locally
---
## Setup Instructions

### 1. Install n8n
```bash
npm install -g n8n
```
### 2. Start n8n
```bash
n8n start
```
Open browser at: `http://localhost:5678`
### 3. Import Workflow
- In n8n, click `...` → `Import from file`
- Select the `.json` file from this repository
### 4. Configure Gmail SMTP Credential
| Field | Value |
|-------|-------|
| Host | `smtp.gmail.com` |
| Port | `465` |
| SSL | Enabled |
| User | your Gmail address |
| Password | Gmail App Password (16 characters) |
> **Note:** Gmail App Password requires 2-Step Verification to be enabled on your Google account. Generate it at `myaccount.google.com/apppasswords`
### 5. Activate Workflow
Click **"Publish"** to activate the schedule.
---
output will be:
<img width="1359" height="608" alt="Screenshot 2026-06-06 231302" src="https://github.com/user-attachments/assets/9c3254d3-006a-4788-a99f-29bb960ab2b5" />

## Course Reference
This project is part of the **AI Automation Course** — learned via YouTube.
