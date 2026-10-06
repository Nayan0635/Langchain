# LangChain

A comprehensive Python project for experimenting, building, and deploying LLM applications using **LangChain** with integrations for OpenAI, Groq, and Google Gemini models.
date- 03-10-2026 time 01:16:46/11:13:25
---

## 📌 Project Overview

This repository serves as a workspace for exploring LangChain concepts, model integrations, prompt templates, and AI agents. It includes hands-on Jupyter notebooks and structured Python scripts.

---

## 🛠️ Features & Integrations

- **Multi-Provider LLM Integration**: Seamless connectivity with **OpenAI**, **Groq**, and **Google Gemini** (`langchain-google-genai`).
- **Environment Management**: Secure API key handling via `python-dotenv`.
- **Interactive Notebooks**: Practical walkthroughs for model initialization, prompt management, and output parsing.
- **Modern Python Tooling**: Dependency management powered by `uv` / `pyproject.toml`.

---

## 📂 Project Structure

```
Langchain/
├── src/
│   └── langchainupdated/        # Core library source code
├── updatedLangchain/            # Interactive Jupyter notebooks & scripts
│   ├── 1-langchainintro.ipynb   # Introduction to LangChain concepts
│   ├── 2-modelintegration.ipynb # Multi-model setup (OpenAI, Gemini, Groq)
│   └── ...
├── .env.example                 # Template for environment variables (excluded from git)
├── .gitignore                   # Excludes secrets (.env) and virtual environments
├── pyproject.toml               # Project dependencies and metadata
├── requirements.txt             # Standard pip requirements file
└── README.md                    # Project documentation
```

---

## 🚀 Getting Started

### 1. Prerequisites

- Python `>= 3.13`
- [uv](https://github.com/astral-sh/uv) (recommended) or standard `pip`

### 2. Environment Setup

Clone the repository and set up a virtual environment:

```bash
# Using uv (recommended)
uv venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
uv sync

# Or using standard pip
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

### 3. API Key Configuration

Create a `.env` file in the root directory (this file is git-ignored for security):

```env
OPENAI_API_KEY=your_openai_api_key_here
GOOGLE_API_KEY=your_google_api_key_here
GROQ_API_KEY=your_groq_api_key_here
NVIDIA_API_KEY=your_nvidia_api_key_here
```

---

## 💻 Usage

Launch Jupyter Notebook to explore the interactive tutorials:

```bash
jupyter notebook
```

Navigate to `updatedLangchain/` to run:

1. `1-langchainintro.ipynb`: LangChain basics & chains.
2. `2-modelintegration.ipynb`: Model provider integration and configuration.

---

## ⚙️ Dependencies

- `langchain`
- `langchain-community`
- `langchain-openai`
- `langchain-groq`
- `langchain-google-genai`
- `python-dotenv`
- `jupyter` / `ipykernel`

---

## 📄 License

This project is licensed under the MIT License.
