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

   * Alternatively, you can use pip:
   
   ```bash
   pip install -r requirements.txt
   ```

3. Try the Interactive System
   * You can use generate_answer() function in the notebook to ask your question, get an aswer, and see the related retrieved documents.
   ```text
   Test Sorusu: What is the capital of Turkey?
   Model Cevabı: Istanbul

   Getirilen Belgeler:

   Belge 1 (Benzerlik: 0.4957, İndeks: 3616):
   İçerik: Question: what country's flag has a moon and star Answer: Turkey

   Belge 2 (Benzerlik: 0.4908, İndeks: 3144):
   İçerik: Question: who claimed a homeland in parts of turkey iran and iraq Answer: Kurdish people

   Belge 3 (Benzerlik: 0.4390, İndeks: 1188):
   İçerik: Question: ancient area of asia minor including aegean islands Answer: Anatolia

   Belge 4 (Benzerlik: 0.4260, İndeks: 4455):
   İçerik: Question: where was the city of troy located at Answer: Anatolia in modern Turkey

   Belge 5 (Benzerlik: 0.4257, İndeks: 4944):
   İçerik: Question: how much territory did the ottoman empire cover Answer: 2,000,000 sq mi
   ```
   * Or you can use interactive_rag() function to try asking many questions to the system.
   * Example Usage:

   ```text
   İnteraktif sistem başlatılıyor...

   ==================================================
   İNTERAKTİF SORU-CEVAP SİSTEMİ
   ==================================================
   Sorularınızı yazın, çıkmak için 'q' veya 'exit' yazın.
   Belgeleri görmek için soru sonuna '!' ekleyin (örn: 'What is DNA?!')
   ==================================================

   Sorunuz: when did they film hot tub time machine!

   Cevap: Fernie Alpine Resort

   Kullanılan Belgeler:

   Belge 1 (Benzerlik: 0.6929, İndeks: 0):
   İçerik: Question: where did they film hot tub time machine Answer: Fernie Alpine Resort

   Belge 2 (Benzerlik: 0.4383, İndeks: 883):
   İçerik: Question: when was fast times at ridgemont high made Answer: 1982

   Belge 3 (Benzerlik: 0.3974, İndeks: 3199):
   İçerik: Question: what year was the future in back to the future Answer: 2015

   Belge 4 (Benzerlik: 0.3795, İndeks: 2003):
   İçerik: Question: when did the cubs win in back to the future Answer: 2015

   Belge 5 (Benzerlik: 0.3531, İndeks: 3495):
   İçerik: Question: time after time song was in what movie Answer: John Tucker Must Die

   Cevap süresi: 14.51 saniye

   Sorunuz: q
   Sistemden çıkılıyor...
   ```

*Note:  This project is currently under development. The final codebase, including a fully functional RAG-enhanced QA system, will be available soon.* 
