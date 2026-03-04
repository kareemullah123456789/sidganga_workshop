# 2-Day Workshop: LLMs, RAG, Agentic AI & MCP

## Prerequisites
- Python 3.10+
- Docker installed and running
- Ollama installed (`https://ollama.com`)
- Basic Python knowledge
- VS Code with Jupyter extension

## Setup Instructions (Run before workshop)
```bash
# Pull required Ollama models
ollama pull llama3.2
ollama pull nomic-embed-text

# Install Python dependencies
pip install langchain langchain-community langchain-ollama
pip install faiss-cpu
pip install chromadb
pip install pypdf
pip install streamlit
pip install mcp
pip install httpx
pip install transformers
pip install sentence-transformers
pip install openai
```

---

## DAY 1 -- Foundations of LLMs & RAG (6 Hours)

### Session 1 (1.5 Hours) -- Foundations of LLMs + Prompt Engineering
**Topics:**
- Evolution: NLP --> Transformers --> LLMs
- Architecture overview (Transformers, Attention mechanism)
- Generative AI vs Traditional ML
- Prompt Engineering fundamentals

**Hands-On:**
- Using Ollama API to generate structured outputs
- Prompt tuning experiments (zero-shot, few-shot, system prompts)
- Output control (temperature, max tokens, formatting)

**Notebook:** `day1/session1_llm_foundations.ipynb`

---

### Session 2 (1.5 Hours) -- Open-Source LLMs with Ollama + Embeddings
**Topics:**
- Using open-source models (Ollama, Hugging Face)
- Tokenization and embeddings
- Fine-tuning vs Prompting
- Vector embeddings in practice

**Hands-On:**
- Load and run models via Ollama
- Generate and visualize embeddings
- Compare performance across prompts
- Mini task: Build a "Resume Analyzer"

**Notebook:** `day1/session2_opensource_llms.ipynb`

---

### Session 3 (2 Hours) -- Retrieval Augmented Generation (RAG)
**Topics:**
- Why LLMs hallucinate
- RAG architecture
- Vector databases (FAISS, ChromaDB)
- Chunking strategies
- LangChain RAG pipeline

**Hands-On:**
- Build: Custom College Chatbot
  - Upload PDF documents
  - Create embeddings
  - Store in FAISS vector database
  - Retrieve + generate answer

**Notebook:** `day1/session3_rag_pipeline.ipynb`

---

### Session 4 (1 Hour) -- MCP: Model Context Protocol (Part 1)
**Topics:**
- What is MCP and why it matters
- MCP architecture (Client/Server/Host)
- MCP tools, resources, and prompts
- Building an MCP server

**Hands-On:**
- Build a custom MCP server with tools
- Test MCP tools locally

**Notebook:** `day1/session4_mcp_intro.ipynb`

---

## DAY 2 -- Agentic AI, MCP & Deployment (6 Hours)

### Session 5 (1.5 Hours) -- Agentic AI with LangChain Agents
**Topics:**
- What is Agentic AI?
- Single-step vs Multi-step reasoning
- Planning, Memory, Tools
- Auto reasoning loops
- LangChain Agents

**Hands-On:**
- Build a Tool-using AI Agent
  - Calculator tool
  - Web search tool (mock)
  - Agent with reasoning chain

**Notebook:** `day2/session5_agentic_ai.ipynb`

---

### Session 6 (1.5 Hours) -- MCP Deep Dive + Agentic Integration
**Topics:**
- MCP client implementation
- Connecting LLM agents to MCP servers
- Docker-based MCP servers
- MCP in production workflows

**Hands-On:**
- Build an MCP client
- Connect LangChain agent to MCP tools
- Run MCP server in Docker

**Notebook:** `day2/session6_mcp_deep_dive.ipynb`

---

### Session 7 (1.5 Hours) -- Multi-Agent Systems
**Topics:**
- Multi-agent collaboration
- Task decomposition
- Planner --> Executor --> Reviewer architecture
- Autonomous workflow design

**Hands-On:**
- Build: AI Research Assistant
  - Agent 1 --> Research
  - Agent 2 --> Summarize
  - Agent 3 --> Critique
  - Final output generator

**Notebook:** `day2/session7_multi_agent.ipynb`

---

### Session 8 (1.5 Hours) -- Capstone Project + Deployment
**Capstone Options (Team-Based):**
- AI Career Mentor Bot
- AI Legal/Policy Q&A System
- AI Interview Preparation Agent
- AI Research Assistant

**Deployment:**
- Build UI with Streamlit
- Deploy on local server
- Live demo by teams

**Notebook:** `day2/session8_capstone_deployment.ipynb`

---

## Assessment Strategy (For 21st March -- 6 Hours)

| Round | Duration | Focus |
|-------|----------|-------|
| Round 1 | 2 Hours | Practical Implementation -- Build a mini RAG system from scratch |
| Round 2 | 2 Hours | Model Improvement -- Reduce hallucination, improve retrieval, optimize prompts |
| Round 3 | 2 Hours | Technical Evaluation -- Viva + Architecture, Debugging, Design new AI agent |

---

## Tech Stack Summary

| Component | Tool |
|-----------|------|
| LLM Runtime | Ollama (llama3.2) |
| Embeddings | nomic-embed-text / sentence-transformers |
| Framework | LangChain |
| Vector DB | FAISS / ChromaDB |
| MCP | Python MCP SDK |
| Containers | Docker |
| UI | Streamlit |
| Notebooks | Jupyter / VS Code |
