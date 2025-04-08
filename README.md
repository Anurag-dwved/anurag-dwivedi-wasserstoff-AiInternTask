# AI Email Assistant with Gemini

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![Gemini](https://img.shields.io/badge/LLM-Google_Gemini-FFCD00)](https://ai.google.dev/)
[![Gmail](https://img.shields.io/badge/Email-Gmail_API-EA4335)](https://developers.google.com/gmail)
[![Slack](https://img.shields.io/badge/Integration-Slack_API-4A154B)](https://api.slack.com/)

An intelligent email automation system that reads, analyzes, and takes action on your emails using Google's Gemini AI.

## ✨ Features

### Smart Email Processing
- Real-time inbox monitoring via Gmail API
- Context understanding with Google Gemini
- Automatic categorization by intent/urgency
- Thread-aware conversation history

### Action Automation
- One-click reply drafting
- Meeting scheduling (Google Calendar)
- Information lookup (Web Search API)
- Priority notifications (Slack)

### Data Management
- Email history storage
- Attachment handling
- Conversation threading

## 🚀 Quick Start

### Prerequisites
- Python 3.10+
- Google Cloud account
- Slack workspace
# Clone repository
git clone https://github.com/anurag-dwivedi-wasserstoff/ai-email-assistant.git
cd ai-email-assistant

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

## 🏗️ Architecture
graph LR
    A[Gmail] --> B[Email Fetcher]
    B --> C[(Database)]
    B --> D[Gemini Analyzer]
    D --> E[Action Router]
    E --> F[Calendar]
    E --> G[Slack]
    E --> H[Reply Generator]
 Project Structure
Copy
email-assistant/
├── .env                    # Environment variables
├── .gitignore              # Git ignore rules
├── venv/                   # Python virtual environment
├── emails.db               # SQLite database
│
├── src/
│   ├── ai_processor.py     # Gemini AI processing
│   ├── calendar_service.py # Calendar integration
│   ├── config.py           # Configuration
│   ├── email_assistant.py  # Main application
│   ├── gmail_service.py    # Gmail API
│   ├── models.py           # Database models
│   └── slack_notifier.py   # Slack notifications
│
├── credentials/
│   ├── credentials.json    # Google OAuth
│   ├── token.json          # Auth token
│   └── client_secret.json  # Client secret
│
└── requirements.txt        # Dependencies

 Requirements
google-generativeai python-dotenv psycopg2 sqlalchemy slack-sdk requests
google-auth google-auth-oauthlib google-api-python-client
