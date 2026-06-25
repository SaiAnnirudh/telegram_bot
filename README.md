# Telegram AI Chatbot with File Analysis

## Overview
This is a Telegram bot that integrates with **Gemini AI** for chat-based interactions and **file analysis**. The bot allows users to:
- Chat with **Gemini AI**
- Upload **PDF, DOCX, TXT, and image** files for text extraction and analysis
- Perform **web searches** using Google Custom Search Engine
- Store and retrieve **chat history** and **file analysis** results using MongoDB

## Features
✅ **Chat with Gemini AI** – Users can send text messages, and the bot replies with AI-generated responses.  
✅ **File Processing** – Supports PDF, DOCX, TXT, and image-based OCR extraction.  
✅ **Web Search** – Fetches search results using Google Custom Search Engine.  
✅ **MongoDB Integration** – Stores user data, chat history, and file analyses.  
✅ **Contact Collection** – Asks users to share their phone numbers for registration.  

## Installation & Setup
### 1️⃣ Prerequisites
Ensure you have the following installed:
- Python 3.8+
- MongoDB
- Telegram Bot API Token
- Google API Key & Custom Search Engine ID

### 2️⃣ Clone the Repository
```sh
git clone https://github.com/your-repo/telegram-bot.git
cd telegram-bot
```

### 3️⃣ Install Dependencies
```sh
pip install -r requirements.txt
```

### 4️⃣ Set Up Environment Variables
Create a **.env** file and add the following:
```sh
TELEGRAM_BOT_TOKEN=your_telegram_bot_token
GEMINI_API_KEY=your_gemini_api_key
MONGO_URI=mongodb://localhost:27017/telegram_bot
GOOGLE_CSE_ID=your_google_cse_id
```

### 5️⃣ Run the Bot
```sh
python bot.py
```

## Bot Commands
| Command | Description |
|---------|-------------|
| `/start` | Register or welcome back users |
| `/websearch <query>` | Search the web for a query |

## File Support & Extraction
The bot can process the following file types:
- **PDF** (Extracts text using PyPDF2)
- **DOCX** (Extracts text using python-docx)
- **TXT** (Reads text directly)
- **Images (JPG, PNG)** (Extracts text using OCR via pytesseract)

## Deployment
To run the bot **24/7**, deploy it on a **VPS** or **cloud platform** like:
- **Heroku**
- **AWS EC2**
- **Google Cloud VM**
- **Railway.app**

Use a process manager like **`screen`**, **`tmux`**, or **`PM2`** to keep it running continuously:
```sh
nohup python bot.py &
```

## Contributing
Feel free to fork this repo and submit pull requests! 🚀
