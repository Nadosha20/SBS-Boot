# SBS Knowledge Assistant 🤖

A Telegram bot built with **n8n** for the **SBS** initiative.
It receives learning material from members and returns a transcript for it.

<img width="701" height="889" alt="Screenshot From 2026-10-30 13-34-32 (Edited)" src="https://github.com/user-attachments/assets/72a59293-5125-4437-a61a-317f18497ee2" />


## What it does
- Welcomes the user and asks which type of data they will send
- Accepts: video links, PDFs, audio, and images
- Gets YouTube transcripts using TranscriptAPI
- Tracks each user's progress in a Postgres database
- Replies to the user directly on Telegram

## Tech stack
| Tool | Usage |
|------|-------|
| n8n | Workflow automation |
| Telegram Bot API | User interface |
| TranscriptAPI | YouTube transcripts |
| PostgreSQL | Storing user progress |

## How to use
1. Open n8n and choose **Import from File**.
2. Select `sbs-knowledge-assistant.json`.
3. Create your own credentials in n8n:
   - Telegram (bot token from @BotFather)
   - Postgres
   - TranscriptAPI (HTTP Header Auth)
4. Create the `progress` table in your database.
5. Activate the workflow and send a message to your bot.

## Note
No secrets are stored in this file. All credentials are kept inside n8n.

## About
This is the last project I built while learning n8n during my journey in SBS.

Built by [Nadosha20](https://github.com/Nadosha20)
