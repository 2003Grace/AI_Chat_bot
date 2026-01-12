# ✈️ Airline Ticket Chatbot  

## 📌 Project Overview  
This project implements a conversational chatbot powered by Gemini/LLM, vector search (RAG) with Qdrant to answer questions, MCP integration for flight search, and an administration interface to manage the knowledge base and statistics to analyze usage..  
(July 2025).  

The chatbot leverages **Large Language Models (LLMs)** and integrates with **Meta’s WhatsApp Business API** to enable natural and interactive communication with users.  

---

## 🚀 Features  
- 🗣️ **Conversational AI**: Handles natural language queries from users.  
- 👥 **Dynamic Context Updates**: Remembers user-provided details (e.g., passengers, dates, destinations) and updates them without restarting the whole search.  
- 📅 **Flight Search**: Retrieves and proposes flight options based on user preferences.
- 📋 **General Informations** : Provide a general overview about the concerned company.
- 🔄 **Webhook Integration**: Connected to Meta Developers for real-time message exchange.  
- 🧪 **User Testing Framework**: Designed with a focus on human–AI interaction for better usability.  

---

## 🛠️ Tech Stack  
- **Language Models**: LLMs for natural language understanding.  
- **Backend**: Python (Flask/FastAPI).  
- **Database**: Mongodb/qdrant for user and document session management.  
- **API Integration**: Meta WhatsApp Business API for communication.  
- **Deployment**: Docker & Ngrok for testing, cloud deployment planned.  

---

## ⚙️ Installation  

1. **Clone the repository**  
```bash
git clone https://github.com/2003Grace/AI_Chat_bot .git
cd AI_Chat_bot 
```

2. **Set up a virtual environment**  
```bash
python -m venv venv
source venv/bin/activate  # On Linux/Mac
venv\Scripts\activate     # On Windows
```

3. **Install dependencies**  
```bash
pip install -r requirements.txt
```

4. **Configure environment variables**  
Create a `.env` file and set your credentials:  
```
WHATSAPP_VERIFY_TOKEN=your verify token
WHATSAPP_ACCESS_TOKEN=your access token
PHONE_NUMBER_ID=your phone number ID


API_BASE_URL = The API for the company. #you can remplace it depending on what you want.

GEMINI_API_KEY=your Gemini API key 

GEMINI_MODEL="gemini-2.5-flash" #you can change depending on which model you want to use



DB_connect = "mongodb+srv://kevine:24446666688888888@mydata.kn4ksk4.mongodb.net/?retryWrites=true&w=majority&appName=mydata"

ADMIN_USERNAME= My AUTH Admin name. #change to your own
ADMIN_PASSWORD= My AUTH Admin password. #change to your own
QDRANT_USE_SERVER=true


ADMIN_ALLOWED_ORIGINS= Cors Config

QDRANT_URL=Server link of the qdrant db

MAX_PDF_SIZE = 15728640  # 15 MB

API_PORT=8001
```

5. **Run the server**  
```bash
python server.py
```
```bash
python whatsapp_travel_bot_test.py
```
```bash
python kb_admin_api.py
```
---

## 📡 Webhook Setup  
- Create a **Meta Developer App** and configure **Webhook URL + Verify Token**.  
- Subscribe to the **messages** endpoint.  
- Replace temporary tokens with a **permanent access token** generated via **system user**.  


---

## 📅 Context  
This project is part of my professional internship (July–December 2025).  
Supervisor requested: **(open for collaboration/mentorship, especially on LLMs & AI agents)**.  

---


## 👨‍💻 Author  
**Kevine Grace**  
- MSc Data Science (AIMS, Cameroon)  
- MSc Physics (Electronics, Electrical Engineering & Automation, University of Dschang)  
- Passion: AI Agents 🤖, Human–AI Interaction, Data-Driven Systems  
