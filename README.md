**Groq-Powered AI Chatbot**

**A Free AI Chatbot Application Utilizing Groq API with a ChatGPT-Style Web Interface**

---

### **Overview**
The Groq-Powered AI Chatbot is a highly efficient and scalable conversational AI solution leveraging Groq's Large Language Model (LLM) API. This project features a Flask-based backend that integrates seamlessly with Groq’s API for intelligent chat responses, complemented by a dynamic, ChatGPT-inspired frontend for an intuitive user experience.

---

### **Key Capabilities**
- **REST API with Flask** for seamless chatbot interactions
- **Groq's LLM API integration** for advanced language understanding
- **Session-based conversation tracking** for continuity
- **Live response streaming** for real-time conversations
- **Modern and responsive web UI** with a ChatGPT-like experience
- **Multiple chat sessions support** with easy management
- **Options to rename and delete conversations**
- **Chat history clearing feature**

---

### **Installation Guide**
#### **Clone the Project Repository:**
```sh
git clone https://github.com/SakibAhmedShuva/Groq-Based-LLM-ChatBot-App.git
cd Groq-Based-LLM-ChatBot-App
```
#### **Install Dependencies:**
```sh
pip install -r requirements.txt
```
#### **Configure API Access:**
1. Create a Groq account and generate an API key.
2. Replace the `api_key` variable in `bot.py` with your Groq API key.

---

### **How to Use**
#### **Run the Flask Server:**
```sh
python bot.py
```
#### **Access the Chat Interface:**
Open `index.html` in your preferred web browser.

---

### **Available API Endpoints**
#### **1. Start a New Chat Session**
- **Endpoint:** `/create-session`
- **Method:** `POST`
- **Response Example:**
```json
{
  "status": "success",
  "session_id": "unique-session-id"
}
```

#### **2. Send and Receive Messages**
- **Endpoint:** `/stream-chat`
- **Method:** `POST`
- **Request Format:**
```json
{
  "session_id": "unique-session-id",
  "messages": [
    {
      "role": "user",
      "content": "User message here"
    }
  ]
}
```
- **Response Example:**
```json
{
  "status": "success",
  "response": "Assistant's response here",
  "history": [
    {
      "role": "user",
      "content": "User message here"
    },
    {
      "role": "assistant",
      "content": "Assistant's response here"
    }
  ]
}
```

#### **3. Clear Conversation History**
- **Endpoint:** `/clear-history`
- **Method:** `POST`
- **Request Format:**
```json
{
  "session_id": "unique-session-id"
}
```
- **Response Example:**
```json
{
  "status": "success",
  "message": "Chat history has been cleared."
}
```

---

### **User Interface Details**
The chatbot includes a ChatGPT-style frontend designed with HTML, CSS, and JavaScript, making it easy to use and integrate.
#### **Highlights:**
- **Fully responsive layout** for desktops and mobile devices
- **Multiple chat session management** (create, rename, delete conversations)
- **Live message streaming** for real-time responses
- **Optional Markdown formatting** for bot replies
- **Chat history clearing option**
- **User-friendly sidebar for session navigation**

---




