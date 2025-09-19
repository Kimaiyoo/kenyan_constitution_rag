# 🇰🇪 Kenyan Constitution RAG with ChatGroq

A **Retrieval-Augmented Generation (RAG)** system that answers questions about the **Kenyan Constitution (2010)**.  
It uses:
- **FAISS** for semantic search  
- **HuggingFace embeddings** for text vectorization  
- **ChatGroq** (`llama-3.1-8b-instant` by default) for context-aware answers

Everything runs inside a Jupyter Notebook for easy experimentation.

---

## 🔧 Setup

Install dependencies:

```bash
pip install -r requirements.txt
```
Create a .env file in the project root:

```env
GROQ_API_KEY=your_api_key_here
```
Get your key from [Groq Console](https://console.groq.com) under API keys.

## 📄 Data
Download The Constitution of Kenya (2010) pdf and place it in the project root.

## ▶️ Usage
1. Open the notebook:
```bash
jupyter notebook Kenyan_Constitution_RAG.ipynb
```
2. Run all cells step by step
3. Ask questions interactively at the end of the notebook.

## ⚙️ Configuration
- Model: llama-3.1-8b-instant (you can switch to mixtral-8x7b-32768)
- Chunk size: 500
- Chunk overlap: 100
- Retriever: Top 3 most relevant chunks

You can tweak these parameters directly in the notebook.

## 🛠 Troubleshooting
- PDF not found: Make sure The_Constitution_of_Kenya_2010.pdf exists in the root directory.
- API key missing: Check .env and reload environment variables.
- FAISS errors: Install faiss-cpu with pip install faiss-cpu.

## 📜 License
- This project is open-sourced under the MIT License.
- The Constitution of Kenya (2010) is a public document.
