# 🤖 AgenticAIChatbot

AgenticAIChatbot is a full-stack conversational agent powered by **LangGraph**, **LangChain**, **Groq LLMs**, and **Tavily Search**. This project offers both an API (FastAPI) and a Streamlit-based frontend to interact with an AI chatbot that dynamically uses ReAct agents and external search tools to respond intelligently.

---

## 🌐 Project URL

GitHub: [AgenticAIChatbot](https://github.com/Aditya26Das/AgenticAIChatbot)

---

## 📁 Folder Structure

```bash
AgenticAIChatbot/
├── api/
│   └── main.py               # FastAPI backend with ReAct agent
├── streamlit_app/
│   └── app.py                # Streamlit frontend for user interaction
├── .gitignore                # Ignore environment, cache, etc.
├── .env                      # API keys and environment variables
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```


---

## 🚀 Features

- ✅ Chat interface powered by **LangGraph ReAct agent**
- 🧠 Supports **multiple LLMs** (LLaMA3, Mixtral) via Groq
- 🔍 Integrated **Tavily Web Search** tool
- 🔄 Real-time responses via API and Streamlit
- 📡 FastAPI-based backend for API access
- 🔒 Environment variable management via `.env`

---

## 🛠️ Tech Stack

| Layer        | Technology                        |
|--------------|------------------------------------|
| Frontend     | Streamlit                          |
| Backend API  | FastAPI                            |
| LLMs         | Groq LLaMA3, Mixtral               |
| Tooling      | LangGraph, Tavily, LangChain       |
| Env Mgmt     | python-dotenv                      |
| Packaging    | pip / requirements.txt             |

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/Aditya26Das/AgenticAIChatbot.git
cd AgenticAIChatbot
```
### 2. Set up a virtual environment

```bash
python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up your .env file

```bash
GROQ_API_KEY=your_groq_api_key
TAVILY_API_KEY=your_tavily_api_key
API_END_POINT=http://127.0.0.1:8000  # or your deployed API URL
```

## Running the App

### 1. Run the FastAPI backend (in api/):

```bash
cd api
uvicorn main:app --reload
```

### 2. Run the Streamlit frontend (in streamlit_app/):

```bash
cd ../streamlit_app
streamlit run app.py
```

## Demo Preview
```bash
| Page                       | Description                   |
| -------------------------- | ----------------------------- |
| 🧠 `Define you AI Agent:`  | Write your system prompt      |
| 💬 `Enter your message(s)` | Send your query to the agent  |
| 🤖 `Agent Response`        | AI's final answer shown below |
```

## Future Improvements
- Chat history storage (Redis / DB)
- Agent memory integration
- More tools like code interpreter, file reader
- OpenAI or Anthropic model support
- Export responses to PDF or Markdown
