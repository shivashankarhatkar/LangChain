# LangChain AI Engineering Toolkit (LangChainP)

An educational and production-ready repository demonstrating the end-to-end lifecycle of Generative AI applications using the LangChain framework. This project systematically breaks down advanced LLM orchestration concepts—from basic prompt templates to complete Retrieval-Augmented Generation (RAG) pipelines—into scalable Python implementations.

---

### 🌟 Business Value & Impact 
* **What it does:** This project acts as a complete blueprint for building intelligent corporate systems. It provides the building blocks that allow an AI model to read massive company databases, structure messy data, and answer customer queries accurately based on company files.
* **Why it matters:** Instead of building simple chatbots that guess answers, this toolkit enables enterprises to automate document analysis, reduce human data-entry labor, and securely search internal proprietary documents with high precision.

---

### 🚀 Module Architecture & Features
The repository is structured sequentially to showcase mastery over the entire LangChain ecosystem:

* **1. LLM Integration & Invocation:** Base configuration for securely initializing, parameterizing (temperature, top_p), and querying state-of-the-art chat models (Demonstrated in `01_llm.ipynb`).
* **2. Advanced Prompt Engineering:** Utilizing `PromptTemplate`, `ChatPromptTemplate`, and dynamic `MessagesPlaceholder` to manage systemic chat history context cleanly (Demonstrated in `02_promptTemplate.ipynb`).
* **3. Structured Output Extraction:** Forcing LLMs to return strict JSON, `TypedDict`, or type-safe `Pydantic` objects instead of raw string text, making outputs ready for application APIs (Demonstrated in `03_Structured_output.ipynb`).
* **4. Output Parsers:** Processing, validating, and formatting raw LLM string results into predictable code execution variables.
* **5. LangChain Chains (LCEL):** Composing modular components into multi-step execution workflows using the LangChain Expression Language.
* **6. Document Loaders:** Extracting raw content from external enterprise data silos like PDFs, Markdown files, Text files, and JSON formats.
* **7. Text Splitters:** Splitting massive documents into semantic, overlapping chunks to fit within LLM context window boundaries.
* **8. Vector Embeddings:** Translating split textual data into highly dense mathematical vector spaces using semantic embedding models.
* **9. Vector Store Databases:** Persisting high-dimensional vector embeddings into local storage indexes (e.g., ChromaDB, FAISS) for lightning-fast lookups.
* **10. Intelligent Retrievers:** Setting up querying pipelines to pull the most contextually relevant document snippets based on user queries (The foundation of RAG).

---

### 🛠️ Tech Stack
* **Orchestration Framework:** LangChain / LangChain Core / LangChain Community
* **Language:** Python 3.10+
* **AI Models:** Google Gemini (`gemini-2.5-flash`)
* **Data Validation:** Pydantic / TypedDict
* **Environment Management:** Python-dotenv

---

### 📦 Quick Setup

1. **Clone the repository:**
```bash
git clone [https://github.com/Shrinath-816/LangChainP.git](https://github.com/Shrinath-816/LangChainP.git)
cd LangChainP

2. **Install dependencies:**
pip install -r requirements.txt

3. **Configure Environment Variables:**Create a .env file in the project root directory and insert your credentials: 
GEMINI_API_KEY=your_gemini_api_key_here
