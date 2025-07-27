
# 🧠 langchain-groq-app

This project demonstrates a minimal LangChain application using **Groq's LPU-powered LLMs** (like LLaMA 3) via `langchain-groq`, built in a Jupyter notebook. The code shows how to invoke a powerful Groq-hosted model using a prompt template pipeline.

---

## ⚙️ Tech Stack

- **LangChain**
- **Groq API (via `langchain-groq`)**
- **LangChain OpenAI (optional)**
- **Jupyter Notebook**
- **uv (Python package manager)**

---

## 📦 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/langchain-groq-app.git
cd langchain-groq-app
````

### 2. Create Environment Using `uv`

```bash
uv venv
source .venv/bin/activate  # or `.venv\Scripts\activate` on Windows
uv pip install -e .
```

If you're just working with the notebook:

```bash
uv pip install langchain-groq langchain python-dotenv langchain-openai ipykernel
```

---

## 🔐 3. Environment Variables

Create a `.env` file in the project root with the following:

```env
GROQ_API_KEY=your_groq_api_key
# Optional: for using OpenAI
OPENAI_API_KEY=your_openai_api_key
```

---

## 📓 4. Run the Notebook

```bash
uv pip install notebook
jupyter notebook
```

Open the notebook and run all cells in order:

```bash
0_langchain_groq_example.ipynb
```

> The model used: `llama-3.3-70b-versatile` via `ChatGroq`

---

## 🧪 5. Example Prompt

```python
question = "Explain LLM like I'm 5."
response = chain.invoke({"question": question})
print(response.content)
```

---

## 🧹 Optional Cleanup

To remove the virtual environment:

```bash
rm -rf .venv
```





---

Let me know if you'd like:
- A version for converting this notebook into a script (`.py`) version
- A Streamlit/Gradio wrapper for interactive UI
- `requirements.txt` auto-generation

I can include that too.

