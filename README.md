# 🤖 Optmizcode AI Assistant

### AI-Powered Chatbot Using Python, FastAPI, LangChain Agents & Ollama

Optmizcode AI Assistant is an AI-powered conversational chatbot developed using **Python, FastAPI, LangChain, LangGraph, and Ollama**.

The chatbot is designed to help website visitors learn about Optmizcode's digital services, including AI-driven development, SEO, digital marketing, branding, and website optimization.

This project demonstrates practical knowledge of **Large Language Models (LLMs), AI Agents, API Development, Prompt Engineering, and Full-Stack AI Integration**.

## 🚀 Key Features

- **AI-Powered Conversations:** Generates responses using a locally running LLM.
- **LangChain Agent Integration:** Uses the LangChain agent framework to manage AI interactions.
- **FastAPI Backend:** Provides REST API endpoints for chatbot communication.
- **Conversation Memory:** Uses LangGraph's InMemorySaver to maintain conversation context.
- **Custom System Prompt:** Defines the assistant's business identity and response guidelines.
- **Interactive Web Interface:** Built using HTML, CSS, and JavaScript.
- **Asynchronous API Requests:** Uses Python async/await and JavaScript Fetch API.
- **New Conversation:** Allows visitors to start a fresh chat session.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend development |
| FastAPI | REST API framework |
| LangChain | LLM and agent orchestration |
| LangGraph | Conversation memory |
| Ollama | Local LLM inference |
| Qwen 2.5 | Language model |
| Pydantic | API input validation |
| HTML, CSS | Frontend interface |
| JavaScript | API communication |

## 🧠 System Architecture

```text
User
  ↓
HTML / CSS / JavaScript
  ↓
FastAPI REST API
  ↓
LangChain Agent
  ↓
Custom System Prompt + Memory
  ↓
Ollama (Qwen 2.5)
  ↓
AI Generated Response
  ↓
FastAPI → Website Chat Interface
```

## ⚙️ Installation & Setup

**1. Clone the repository**

```bash
git clone <your-repository-url>
cd <your-repository-folder>
```

**2. Install dependencies**

```bash
pip install fastapi uvicorn langchain langchain-ollama langgraph
```

**3. Install Ollama and download the model**

```bash
ollama pull qwen2.5:3b
```

**4. Start the FastAPI server**

```bash
python -m uvicorn assistance:app --reload
```

**5. Open the chatbot**

```text
http://127.0.0.1:8000
```

## 💬 API Example

**Endpoint:** `POST /chat`

Request:

```json
{
  "message": "What SEO services does Optmizcode provide?",
  "thread_id": null
}
```

Example response:

```json
{
  "thread_id": "generated-conversation-id",
  "response": "Optmizcode provides SEO and digital marketing services to help businesses improve their online visibility."
}
```

The API returns a conversation ID, allowing subsequent messages to continue the same conversation.

## 🎯 Project Objective

The goal of this project is to develop a practical AI chatbot that combines modern LLM technologies with backend API development and a user-friendly web interface.

It also serves as a foundation for exploring more advanced concepts such as Retrieval-Augmented Generation (RAG), vector databases, advanced tool calling, and production AI deployment.

## 👨‍💻 Developer

**Sadat Ali Khan**

Python | FastAPI | Machine Learning | AI Development

- GitHub: [sadatalikhan122](https://github.com/sadatalikhan122)
- LinkedIn: [Sadat Ali Khan](https://www.linkedin.com/in/sadat-ali-khan-90ba701a0/)

---

*Built as a hands-on project to explore LLM integration, AI agents, and full-stack AI application development.*
