# VeriDoc AI ⚖️
**A Verifiable Enterprise Legal & Corporate Policy Copilot**

VeriDoc AI is a robust, purely Python-based Retrieval-Augmented Generation (RAG) system designed to safely analyze complex legal contracts and corporate policies. In high-stakes enterprise environments, standard LLMs pose a massive liability due to factual hallucinations. VeriDoc AI eliminates this risk by employing a strict **Dual-Agent Architecture**. 

When a user queries a document, a **Generator Agent** drafts the response, while a separate **Verifier Agent** cross-references that draft against the original source text. Any claim not explicitly backed by the uploaded document is instantly blocked or rewritten, guaranteeing zero-hallucination factual accuracy.

## ✨ Core Architecture & Features
* **Dual-Agent Verification:** An automated human-in-the-loop-style safety mechanism that prevents the AI from fabricating legal clauses or citing non-existent policies.
* **High-Throughput Ingestion:** Fast, asynchronous document processing, text chunking, and vector embedding built on **FastAPI**.
* **Semantic Search:** Low-latency querying and context retrieval using **PostgreSQL** paired with the **pgvector** extension.
* **Translation Support**: Translate answers into multiple languages including Urdu, Hindi, Spanish, and French.
* **Text-to-Speech**: Generate audio responses for the translated answers.
* **User -Friendly Interface**: Built with Streamlit for an interactive user experience.


## Installation
1. **Install the required packages**:
  ```
   pip install -r requirements.txt
  ```
2. **Set up your API key**:
   - Obtain your API key from Groq and set it as an environment variable
3. **Run the app locally**:
```
   streamlit run app.py
```
## Usage

1. **Upload a Document**: Use the file uploader to upload a PDF or TXT document.
2. **Ask Questions**: Enter your questions in the provided input field.
3. **Select Translation Options**: Choose a language for translation if needed.
4. **Receive Answers**: View the AI-generated answers and listen to audio playback if enabled.

---
*Copyright © 2026 Rishi Raj Anand*
