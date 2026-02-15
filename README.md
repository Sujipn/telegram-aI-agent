# 🤖 Telegram Conversational AI Assistant

## 📌 Overview
This project implements a **Telegram-based conversational AI assistant** powered by Google Gemini.

The assistant receives messages from Telegram users, processes them using an AI agent with memory and tools, and sends intelligent responses back in real time.

It supports:

- 💬 Natural conversation
- 🧠 Context-aware memory per user session
- 🌐 Web/context search via Gemini Search Tool
- 🕒 Date & time awareness
- 📩 Instant Telegram replies

This workflow demonstrates how to build a **production-style AI chatbot integrated with messaging platforms**.

---

## 🧠 Architecture

### **Message Flow**


Telegram Trigger → AI Agent → Telegram Response


### **AI Agent Components**

- **Google Gemini Chat Model** — generates responses
- **Memory Buffer Window** — maintains chat history per Telegram user
- **Gemini Search Tool** — retrieves external context when needed
- **Date & Time Tool** — enables time-aware responses

Each Telegram chat ID is used as a **session key**, ensuring conversations remain contextual for every user.

---

## ✨ Features

- ✅ Real-time Telegram chatbot  
- ✅ Context-aware multi-turn conversations  
- ✅ Google Gemini LLM integration  
- ✅ External search capability  
- ✅ Date & time tool support  
- ✅ Session-based memory handling  
- ✅ HTML-formatted Telegram responses  

---

## 🛠️ Requirements

- Telegram Bot Token  
- Google Gemini API key  
- Gemini Search API credentials (optional but recommended)  
- n8n (latest version recommended)  

---

## 🔑 Setup Instructions

### 1️⃣ Create Telegram Bot
1. Open Telegram  
2. Search for **@BotFather**  
3. Run `/start` → `/newbot`  
4. Copy the generated **Bot Token**

---

### 2️⃣ Import Workflow
1. Open n8n  
2. Import the provided JSON workflow file  
3. Save the workflow

---

### 3️⃣ Configure Credentials

Update credentials in:

- **Telegram Trigger**
- **Send a text message node**
- **Google Gemini Chat Model**
- **Gemini Search Tool (optional)**

---

### 4️⃣ Activate the Workflow

1. Enable the workflow  
2. Send a message to your Telegram bot  
3. The AI assistant will respond automatically

---

## 💬 Example Queries

Try asking your bot:

- What is machine learning?
- What time is it now?
- Summarize the latest AI news
- Explain Python decorators simply


---

## 📂 Workflow Components

| Node | Purpose |
|------|--------|
| Telegram Trigger | Receives incoming user messages |
| AI Agent | Core reasoning engine orchestrating tools |
| Gemini Chat Model | Generates conversational responses |
| Memory Buffer | Stores session chat history |
| Gemini Search Tool | Provides external context retrieval |
| Date & Time Tool | Supplies current date/time info |
| Send Telegram Message | Sends response back to user |

---

## 🧩 How It Works

1. User sends a message on Telegram  
2. Trigger captures the message and chat ID  
3. AI agent processes input using Gemini  
4. Agent uses memory/tools if needed  
5. Response is returned to Telegram instantly  

---

## 🚀 Possible Improvements

- Add knowledge base / vector database (RAG)
- Store conversations in database
- Add voice message support
- Connect to Slack / WhatsApp
- Add moderation & safety filters
- Deploy with public webhook endpoint

---

## 📜 License

This project is provided for **learning and portfolio demonstration purposes**.

---

## 🙌 Credits

Built using:

- **Telegram Bot API**
- **Google Gemini**
- **n8n**

---

## 📬 Contact
If you'd like to discuss this project or my experience:  
📧 **Email:** sujipn@gmail.com  
🔗 **LinkedIn:** http://linkedin.com/in/sujitha-pathmanathan
