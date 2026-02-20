# Automation-Email


Telegram AI Email Assistant (n8n Workflow)

Project Overview

An AI-powered email assistant built using n8n, Telegram Bot, OpenAI Chat
Model, and Gmail API.

This workflow allows users to interact via Telegram to:

-   Summarize emails
-   Send emails
-   Summarize and send emails
-   Receive structured execution reports

Architecture Overview

Components:

1.  Telegram Trigger – Captures user messages
2.  AI Agent (LangChain) – Understands user intent
3.  OpenAI Chat Model (gpt-5-mini) – Processes natural language
4.  Gmail Tool (Get) – Fetches emails
5.  Gmail Tool (Send) – Sends emails
6.  Telegram Node – Sends execution report back

Workflow Logic

1.  User sends a message via Telegram.
2.  The AI Agent interprets the request.
3.  Based on intent, the system:
    -   Retrieves emails
    -   Summarizes emails
    -   Sends an email
    -   Or performs both actions
4.  The assistant returns a structured execution report.

Output Format

Task Performed: Email Summary / Email Sent / Email Summary & Sent

Details: Short factual description

Status: Success

Design Rules

-   No greetings
-   No reasoning explanation
-   No email content unless explicitly requested
-   Only execution report returned

Tech Stack

-   n8n (Workflow Automation)
-   OpenAI Chat Model (gpt-5-mini)
-   Gmail API (OAuth2)
-   Telegram Bot API
-   LangChain Agent Node

Required Credentials

-   Telegram Bot API credentials
-   Gmail OAuth2 credentials
-   OpenAI API credentials

All credentials are securely managed inside n8n.

Setup Instructions

1.  Install n8n npm install -g n8n

2.  Import Workflow

    -   Open n8n
    -   Go to Workflows
    -   Click Import
    -   Upload the provided JSON file

3.  Configure Credentials

    -   Set Telegram credentials
    -   Set Gmail OAuth2 credentials
    -   Set OpenAI API credentials

4.  Activate Workflow Toggle the workflow to Active.

Use Cases

-   Personal email automation
-   Executive assistant bot
-   Gmail summarization tool
-   Telegram-based productivity bot
-   AI workflow orchestration demo

Project Status

-   Workflow Designed
-   AI Integration Complete
-   Gmail Integration Complete
-   Telegram Integration Complete
-   Ready for Deployment

Future Improvements

-   Add memory/context tracking
-   Add multi-user access control
-   Add logging and analytics
-   Add attachment summarization
-   Add voice message support

License

MIT License
