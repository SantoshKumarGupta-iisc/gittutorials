
# 💼 Multi-Agent AI Assistant using Phi, Groq, OpenAI, and FastAPI

This project is a powerful **AI agent system** built using [Phi](https://docs.phidata.com/), integrating:
- 📊 **Financial analysis** (with live stock price, fundamentals, and analyst recommendations via `yFinance`)
- 🌐 **Web search capabilities** (using `DuckDuckGo`)
- ⚙️ Backed by **Groq LLaMA 3**, **OpenAI**, and **FastAPI Playground**

---

## 🚀 Features

- 🔍 **Web Search Agent** — searches the web and provides source-backed results.
- 📈 **Finance Agent** — gives real-time stock data, company news, and analyst recommendations.
- 🤝 **Multi-Agent Collaboration** — agents work together to fulfill complex queries.
- 🖥️ **Web Playground UI** — interact with agents in a clean FastAPI interface.
- 🔐 **Secure API management** — keys managed via `.env` and `python-dotenv`.

---

## 🧠 Powered By

| Service     | Usage                                      |
|-------------|--------------------------------------------|
| [Phi](https://docs.phidata.com/)        | Agent framework + tools                 |
| [Groq](https://console.groq.com/)       | LLaMA 3 backend model (ultra fast)      |
| [OpenAI](https://platform.openai.com/) | Optional backend model                  |
| [DuckDuckGo](https://duckduckgo.com/)  | Web search tool                         |
| [Yahoo Finance](https://finance.yahoo.com/) | Stock prices, news, recommendations |
| [FastAPI](https://fastapi.tiangolo.com/) | Playground interface                    |

---

## 🧰 Setup Instructions

### 1️⃣ Clone this repo

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2️⃣ Install dependencies

Make sure you are using Python 3.9+

```bash
pip install -r requirements.txt
```

<details>
<summary>📦 Required packages</summary>

```
phidata
python-dotenv
yfinance
duckduckgo-search
fastapi
uvicorn
groq
openai
packaging
```
</details>

---

### 3️⃣ Create your `.env` file

Create a `.env` file in the root directory:

```env
PHI_API_KEY=your_phi_api_key
GROQ_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
```

> **Warning**: Never expose this file publicly!

---

### 4️⃣ Run the FastAPI Playground

```bash
python your_script_name.py
```

Then go to:  
**http://127.0.0.1:8000/**  
and start chatting with your agents!

---

## 🧪 Sample Query

Try this in the playground:

> `Summarize analyst recommendation and share the latest news for NVDA`

- You'll get a clean table of analyst sentiment.
- Latest stock news.
- All web links and data sources shown.

---

## 📂 Project Structure

```text
.
├── agents.py              # Agent definitions
├── main.py                # Playground launch
├── .env                   # API keys (not committed)
├── requirements.txt       # Dependencies
├── README.md              # You're reading this!
```

---

## ✅ To Do

- [ ] Add logging and error handling
- [ ] Dockerize the project
- [ ] Deploy on Render/Vercel/Streamlit
- [ ] Add UI enhancements (dark mode, chat memory)

---

## 🛡️ Security Note

> 🚨 **API Keys Warning**  
Never commit `.env` files or share your keys publicly.  
Always rotate your keys if accidentally exposed.

---

