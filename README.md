# Mental Health FAQ Chatbot

A question-answering chatbot built using **LangChain**, **Together AI's Mistral LLM**, and **Gradio**.  
This project enables users to ask mental health-related questions and receive detailed answers extracted from a curated FAQ dataset.

<img width="1470" alt="Screenshot 2025-06-08 at 12 00 06 PM" src="https://github.com/user-attachments/assets/a29d74b0-2019-4eec-b5fb-e7610f5aa17f" />

---
## Features

- Retrieves relevant documents from a mental health FAQ dataset using vector search.
- Uses a custom prompt template to generate accurate, context-based answers.
- Powered by the **Mistral Mixtral-8x7B** language model hosted on Together AI.
- Interactive UI built with **Gradio** for easy user interaction.
- Runs seamlessly on **Google Colab** without local installations.

---

## Technologies Used

- LangChain  

- Together AI (Mistral LLM) [Model used: `mistralai/Mixtral-8x7B-Instruct-v0.1`]  

- HuggingFace Embeddings  [Model used: `all-MiniLM-L6-v2`]

- FAISS (Facebook AI Similarity Search)  

- Gradio  
---

## How It Works

1. **Data loading:** FAQ data is loaded from a CSV file.  
2. **Embedding:** Questions are embedded using HuggingFace embeddings.  
3. **Indexing:** Vectors are indexed with FAISS for fast retrieval.  
4. **RetrievalQA chain:** Uses LangChain to create a pipeline combining document retrieval and LLM answer generation with a custom prompt.  
5. **User Interface:** A Gradio interface lets users type questions and get answers from the chain.

---
