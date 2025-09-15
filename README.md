# ChatBot-using-LangGraph

"""# 🤖 LangGraph Chatbot with Streamlit UI

An interactive **Generative AI chatbot** built using **LangGraph** and **Streamlit**, featuring persistent chat storage, multi-session handling, and a clean ChatGPT-like sidebar for navigating previous conversations.

---

## 🚀 Features

- **Multi-session chat**: Start a **new chat** anytime and revisit old ones (sessions displayed as `session-1`, `session-2`, etc.).
- **Persistent storage**: Chats are saved using **SQLite** (`SqliteSaver`) so history is retained even after restarting.
- **Sidebar navigation**: A non-collapsible **sidebar on the left**, showing all active sessions with the latest user message or session number.
- **Simple & clean UI**: Chat interface similar to ChatGPT with smooth session switching.

---

## 🛠️ Tech Stack

- [LangGraph](https://github.com/langchain-ai/langgraph) – for conversation flow and state management.
- [LangGraph Checkpoint SQLite](https://pypi.org/project/langgraph-checkpoint-sqlite/) – for saving chat history.
- [Streamlit](https://streamlit.io) – for frontend UI.
- [SQLite3](https://www.sqlite.org/index.html) – for lightweight local storage.

---

## 📂 Project Structure

.
├── .env (paste your keys)
├── requirements.txt
├── 01_ChatBot_with_memory_checkpoint.ipynb # Jupyter Notebook for experimentation
│
├── ChatBot_backend.py # Backend (memory only)
├── Streamlit_ChatBot_frontend.py # Streamlit frontend (memory only)
├── Streamlit_Chatbot_frontend_UI_1.png # Screenshot for above pair
│
├── ChatBot_database_backend.py # Backend (with SQLite database)
├── Streamlit_frontend_database.py # Streamlit frontend (with SQLite DB)
├── Streamlit_frontend_database_UI_2.png # Screenshot for above pair
│
├── chatbot_memory.db # SQLite database (generated after running DB frontend)
│
├── LICENSE
└── README.md


2️⃣ Create virtual environment
python -m venv lgraph
source lgraph/bin/activate   # Mac/Linux
lgraph\Scripts\activate      # Windows

3️⃣ Install dependencies
pip install -r requirements.txt


