# 🧬 Fine-tuned LLM for Noonan Syndrome

### An AI-powered Semantic Search & Q&A System for Rare Genetic Diagnosis  
_Leveraging Meta LLaMA 3 + FastEmbed on Clinical & Genetic Data_

---

## 📖 Overview

**Fine-tuned-LLM-for-Noonan-Syndrome** is a semantic search-based medical assistant designed to aid in the diagnosis, understanding, and personalized treatment of **Noonan Syndrome**, a complex genetic disorder.  
It utilizes **Meta LLaMA 3**, **FastEmbed** (`BAAI/bge-small-en-v1.5`), and **LlamaIndex** to retrieve and reason over diverse medical datasets including clinical records, genetic mutations, and scientific literature.

> This project demonstrates the potential of large language models (LLMs) in rare disease research, bridging genetic insights with practical clinical decision-making.

---

## 🧠 Key Features

- 🔍 **Semantic Search-Enhanced Q&A** using `LlamaIndex` and vector embeddings
- 💡 **Context-aware Answer Generation** using Meta-LLaMA-3-8B-Instruct
- 🧾 **Multimodal Ingestion** of CSVs, PDFs, and structured clinical records
- ⚙️ **FastEmbed Model Integration** for efficient, low-resource embedding
- 💬 **Gradio Chat Interface** for real-time, interactive querying
- 📊 **Cosine Similarity & F1 Scoring** for evaluation of AI output quality

---

## 🏗️ Architecture

### **Ingestion Pipeline**
1. Upload documents (e.g., `dataformoonan.csv`)
2. Text chunking and preprocessing
3. Embedding with `BAAI/bge-small-en-v1.5`
4. Store vectors in a local vector DB

### **Query Engine**
1. User submits a medical question
2. Query embedding is generated
3. Most relevant text chunks are retrieved via cosine similarity
4. Meta LLaMA 3 generates a final response using the retrieved context

---

