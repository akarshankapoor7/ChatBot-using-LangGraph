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
