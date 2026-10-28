# LLM App Dev Playground

A hands-on Python workspace for learning and experimenting with modern LLM application frameworks — starting with **LangChain**, and expanding over time to **LangGraph**, **RAG**, **vector-less RAG**, **guardrails**, **evals**, and more. Built around interactive Jupyter notebooks with multi-provider model integrations (OpenAI, Groq, Google Gemini, NVIDIA).

> Note: this repo is currently named after LangChain but will be renamed as its scope grows.

---

## 📌 Overview

This is a living, growing reference for building LLM-powered applications — not a single-framework tutorial. Each topic gets its own notebooks/folder as it's added, so the structure below will expand over time.

**Currently covered:**

- LangChain fundamentals (models, messages, tools, structured output, middleware)

**Planned additions:**

- LangGraph (stateful/multi-agent workflows)
- RAG (retrieval-augmented generation)
- Vector-less RAG approaches
- Guardrails / safety & validation layers
- Evals (testing and benchmarking LLM outputs)

---

## 🛠️ Features & Integrations

- **Multi-provider LLM access**: OpenAI, Groq, Google Gemini, NVIDIA NIM
- **Secure config**: API keys via `.env` / `python-dotenv`
- **Interactive notebooks**: practical, runnable walkthroughs for each concept
- **Modern tooling**: dependency management via `uv` / `pyproject.toml`

---

## 📂 Project Structure

```structure
.
├── src/                     # Core reusable library code
├── updatedLangchain/        # LangChain notebooks (models, tools, messages, structured output, middleware)
├── (future) langgraph/      # LangGraph notebooks
├── (future) rag/            # RAG & vector-less RAG notebooks
├── (future) guardrails/     # Guardrails / validation notebooks
├── (future) evals/          # Evaluation & benchmarking notebooks
├── .env.example             # Template for environment variables
├── pyproject.toml           # Project dependencies & metadata
├── requirements.txt         # Pip requirements
└── README.md
```

---

## 🚀 Getting Started

**Prerequisites:** Python ≥ 3.13, [uv](https://github.com/astral-sh/uv) (recommended) or pip

```bash
# Using uv (recommended)
uv venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
uv sync

# Or using pip
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

**API keys** — create a `.env` file (git-ignored) in the root:

```env
OPENAI_API_KEY=...
GOOGLE_API_KEY=...
GROQ_API_KEY=...
NVIDIA_API_KEY=...
```

**Run the notebooks:**

```bash
jupyter notebook
```

---

## ⚙️ Core Dependencies

`langchain` · `langchain-openai` · `langchain-google-genai` · `langchain-groq` · `langchain_nvidia_ai_endpoints` · `python-dotenv` · `jupyter`

(Additional dependencies will be added as LangGraph, RAG, guardrails, and evals sections come online.)

---

## 📄 License

MIT
