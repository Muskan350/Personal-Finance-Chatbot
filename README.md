# Personal-Finance-Chatbot
Built an AI-powered Personal Finance Chatbot using Flask, LangChain, FAISS, and Hugging Face LLM with RAG for personalized financial insights. Automated expense categorization and created Plotly dashboards for spending analysis. Implemented semantic search with FAISS for context-aware Q&amp;A.
# 💰 Personal Finance Chatbot

An AI-powered **Personal Finance Chatbot** that helps users analyze spending habits, categorize expenses, visualize financial data, and receive personalized financial insights through natural language conversations.

The application combines **Flask**, **LangChain**, **FAISS**, **OpenAI Embeddings**, **Hugging Face LLM**, **Ollama**, and **Plotly Dashboard** to deliver intelligent financial assistance while processing user financial data locally whenever possible.

---

## 🚀 Features

- Upload and analyze CSV bank statements
- Automatically categorize financial transactions
- Interactive AI chatbot for financial queries
- Retrieval-Augmented Generation (RAG) using LangChain
- FAISS vector database for semantic search
- Expense categorization using LLMs
- Interactive Plotly dashboard
- Monthly expense visualization
- Expense breakdown by category
- Local execution for improved privacy
- Simple Flask-based web interface

---

## 📊 Dashboard Preview

The dashboard provides:

- Monthly Expense Analysis
- Expense Breakdown by Category
- Interactive Charts
- Spending Trend Visualization

Example:

- 📈 Expense per Month (Bar Chart)
- 🥧 Expense Breakdown by Category (Pie Chart)

---

## 🏗️ Project Architecture

```
                    User
                      │
                      ▼
             Flask Web Interface
             (bot_1.html + Flask)
                      │
                      ▼
                User Question
                      │
                      ▼
             LangChain Pipeline
                      │
      ┌───────────────┴───────────────┐
      ▼                               ▼
Financial Analysis File          User Query
      │                               │
      └───────────────┬───────────────┘
                      ▼
             Text Chunking
 (RecursiveCharacterTextSplitter)
                      │
                      ▼
          OpenAI Embeddings
                      │
                      ▼
             FAISS Vector Store
                      │
                      ▼
           Similarity Search (RAG)
                      │
                      ▼
      Hugging Face Language Model
          (Zephyr-7B Beta)
                      │
                      ▼
           Financial Response
                      │
                      ▼
               User Interface

────────────────────────────────────

CSV Financial Data
        │
        ▼
categorize_expenses.ipynb
        │
        ▼
Expense Categorization
        │
        ▼
dashboard.ipynb
        │
        ▼
Interactive Plotly Dashboard
```

---

# 📁 Project Structure

```
Personal-Finance-Chatbot/

│── chatbot.py
│── bot_1.html
│── dashboard.ipynb
│── categorize_expenses.ipynb
│── requirements.txt
│── complete_financial_analysis.txt
│── README.md
```

---

# 🛠 Technologies Used

### Programming

- Python
- HTML

### AI & Machine Learning

- LangChain
- Retrieval-Augmented Generation (RAG)
- OpenAI Embeddings
- Hugging Face LLM
- Ollama

### Backend

- Flask

### Vector Database

- FAISS

### Visualization

- Plotly

### Notebook

- Jupyter Notebook

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/personal-finance-chatbot.git

cd personal-finance-chatbot
```

Install dependencies

```bash
pip install -r requirements.txt
```

Install Ollama

```bash
ollama pull llama2
```

Run transaction categorization

```bash
jupyter notebook categorize_expenses.ipynb
```

Generate dashboard

```bash
jupyter notebook dashboard.ipynb
```

Run chatbot

```bash
python chatbot.py
```

Open browser

```
http://127.0.0.1:5000
```

---

# 🔑 Environment Variables

Configure the following API keys before running:

```
OPENAI_API_KEY=your_openai_key

HUGGINGFACE_API_KEY=your_huggingface_key
```

---

# 📌 Workflow

1. Upload financial CSV statements.
2. Categorize transactions using AI.
3. Generate interactive financial dashboard.
4. Convert financial analysis into embeddings.
5. Store embeddings inside FAISS.
6. Retrieve relevant financial information using RAG.
7. Generate intelligent responses using Hugging Face LLM.
8. Display responses in the chatbot interface.

---

# 📈 Dashboard Insights

The dashboard includes:

- Monthly spending
- Expense distribution
- Category-wise analysis
- Financial trend visualization

---

# 📚 Learning Outcomes

This project helped in learning:

- Retrieval-Augmented Generation (RAG)
- LangChain pipelines
- FAISS vector databases
- OpenAI Embeddings
- Hugging Face LLM integration
- Flask web development
- Plotly dashboard creation
- Expense categorization using AI
- Financial data visualization

---

# 🔮 Future Enhancements

- PDF bank statement support
- Voice-enabled chatbot
- Multi-language support
- Budget recommendation engine
- Investment suggestions
- Expense prediction using Machine Learning
- Mobile application
- User authentication
- Cloud deployment

---

# 📄 Disclaimer

This project is intended for educational purposes only. Financial advice generated by the chatbot should not be considered professional financial consultation.
