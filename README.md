# anurag-dwivedi-wasserstoff-AiInternTask
# AI Personal Email Assistant 

An intelligent email automation system that reads, analyzes, and takes action on your emails using Google's Gemini AI, with integrations for Slack, web search, and calendar scheduling.
# AI Personal Email Assistant with Gemini

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Gemini](https://img.shields.io/badge/LLM-Google_Gemini-FFCD00)](https://ai.google.dev/)
[![Gmail](https://img.shields.io/badge/Email-Gmail_API-EA4335)](https://developers.google.com/gmail)
[![Slack](https://img.shields.io/badge/Integration-Slack_API-4A154B)](https://api.slack.com/)

An intelligent email automation system that reads, analyzes, and takes action on your emails using Google's Gemini AI.

## ✨ Features

- **Smart Email Processing**
  - Real-time inbox monitoring via Gmail API
  - Context understanding with Google Gemini
  - Automatic categorization by intent/urgency
  - Thread-aware conversation history

- **Action Automation**
  - One-click reply drafting
  - Meeting scheduling (Google Calendar)
  - Information lookup (Web Search API)
  - Priority notifications (Slack)

- **Data Management**
  - Email history storage
  - Attachment handling
  - Conversation threading

## 🏗️ Architecture
graph LR
    A[Gmail] --> B[Email Fetcher]
    B --> C[(Database)]
    B --> D[Gemini Analyzer]
    D --> E[Action Router]
    E --> F[Calendar]
    E --> G[Slack]
    E --> H[Reply Generator]
email-assistant/
├── .env # Environment variables
├── .gitignore # Git ignore rules
├── venv/ # Python virtual environment
├── emails.db # SQLite database file
│
├── src/
│ ├── ai_processor.py # Gemini AI processing logic
│ ├── calendar_service.py # Google Calendar integration
│ ├── config.py # Configuration settings
│ ├── email_assistant.py # Main application entry point
│ ├── gmail_service.py # Gmail API interactions
│ ├── models.py # Database models
│ ├── slack_notifier.py # Slack notification handler
│
├── credentials/
│ ├── credentials.json # Google OAuth credentials
│ ├── token.json # Authentication token
│ └── client_secret_*.json # Client secret file
│
└── requirements.txt # Python dependencies
 Quick Start
##some library installation 
pip install google-generativeai python-dotenv psycopg2 sqlalchemy slack-sdk requests
pip install  google-genai
pip install -q -U google-genai
pip install python-dotenv google-auth google-auth-oauthlib google-api-python-client openai slack-sdk sqlalchemy
source venv/bin/activate # for environment
python src/email_assistant.py 
#clone repository
git clone https://github.com/yourusername/email-assistant.git
cd email-assistant

google cloud console - https://console.cloud.google.com/home/dashboard?invt=AbuMrg&project=freeemailassistant
This project demonstrates how AI-powered automation can transform email management, saving time and improving productivity. With its modular design and clear documentation, it serves as a strong foundation for further development.


