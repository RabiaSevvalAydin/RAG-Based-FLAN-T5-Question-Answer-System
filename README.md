# RAG Based FLAN-T5 Q&A System

This project demonstrates a RAG (Retrieval-Augmented Generation) approach using FLAN-T5, initially developed for academic exploration in advanced LLM principles. It is designed to leverage the power of large language models with efficient retrieval techniques to provide accurate answers to user questions.

## Project Overview
This project implemets a Retrieval-Augmented Generation (RAG) system using:
* Retriever: FAISS 
* LLM Model: FLAN-T5 Large
* Word Embedding: all-mpnet-base-v2
* Dataset: NaturalQuestions
* Evalutaion: EM (Exact Match), F1-score, ROUGE

## Quickstart: Setup & Test The Q&A System
### Prerequisites
- Python 3.10+
- Conda (Recommended for environment management)

1. Clone the repository
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
2. Create a virtual environment
   ```bash
   conda env create -f environment.yml
   conda activate llm_rag_env
   ```
   Alrenatively, use pip:
   ```bash
   pip install -r requirements.txt
   ```
3. Try the Interactive System


🚀 *Note:  This project is currently under development. The final codebase, including a fully functional RAG-enhanced QA system, will be available soon.* 
