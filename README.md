# Product Query Agent

A beginner-friendly **AI agent** tutorial that answers product questions using custom Python tools, a simple in-memory catalog, and conversation memory.

The full walkthrough lives in [`src/code.ipynb`](src/code.ipynb). You will build an agent step by step that:

- Looks up **prices and descriptions** from a product catalog
- Fetches **customer reviews** with a second tool
- Remembers context across turns using **LangGraph memory**

Powered by [LangChain](https://python.langchain.com/), [Groq](https://groq.com/) (`llama-3.1-8b-instant`), and [LangGraph](https://langchain-ai.github.io/langgraph/).

## What you need

- Python **3.10+**
- [pip](https://pip.pypa.io/) (included with Python)
- A free [Groq API key](https://console.groq.com/)

## Setup

### 1. Clone the repository

```bash
git clone https://github.com/YashMehetre/Product-Query-Agent.git
cd Product-Query-Agent
```

No Git? Download the repo as a ZIP from GitHub and unzip it.

### 2. Install dependencies

From the project root (the folder that contains `requirements.txt`):

```bash
pip install -r requirements.txt
```

If `pip` is not found:

```bash
python -m pip install -r requirements.txt        # Windows
python3 -m pip install -r requirements.txt       # macOS / Linux
```

### 3. Add your API key

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key_here
```

This file is listed in `.gitignore` — do not commit or share your key.

## Run the notebook

Open [`src/code.ipynb`](src/code.ipynb) and run the cells **from top to bottom**.

**Option A — Jupyter (browser)**

```bash
jupyter notebook
```

Navigate to `src` → `code.ipynb`.

**Option B — VS Code / Cursor**

Open the **entire project folder** (not just the notebook file), open `src/code.ipynb`, select your Python interpreter, and run the cells.

## Project structure

```
Product-Query-Agent/
├── requirements.txt    # Python dependencies
├── .env                  # Your Groq API key (create this)
└── src/
    └── code.ipynb        # Tutorial notebook — start here
```

## Troubleshooting

| Issue | Fix |
|-------|-----|
| `pip` not found | Use `python -m pip install -r requirements.txt` |
| `GROQ_API_KEY` not set | Ensure `.env` is in the project root and Cell 1 has been run |
| `.env` not loading in VS Code | Open the whole `Product-Query-Agent` folder, not only the `.ipynb` file |
| `No module named 'langgraph'` | Run `pip install langgraph` or reinstall from `requirements.txt` |

## Author

**Mehetre Yash Pritam**

- GitHub: [@YashMehetre](https://github.com/YashMehetre)
- LinkedIn: Yash Mehetre
- Email: mehetreyash12@gmail.com
