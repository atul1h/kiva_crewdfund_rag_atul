# Crowdfunding Insights using Retrieval-Augmented Generation (RAG)

This project implements a **Retrieval-Augmented Generation (RAG) system** to analyze open-source crowdfunding data and generate insights using **open-source embedding models** and a **Groq-hosted LLM**.

---

## Objective

Build a RAG-based system that:
- Processes crowdfunding data
- Creates semantic documents from the data
- Retrieves relevant documents using embeddings
- Generates insights using an open-source language model

---

## Dataset

A **sample Kickstarter crowdfunding dataset** is used.

### Columns Used
- `name` – Project title  
- `category_name` – Project category  
- `goal` – Funding goal (USD)  
- `usd_pledged` – Amount pledged (USD)  
- `state` – Project outcome (successful / failed)  

---

Steps:
1. Removed duplicate rows
2. Dropped rows with missing values
3. Standardized text fields (lowercase)
4. Computed funding ratio
5. Grouped projects by category
6. Created summarized documents for RAG

### Example RAG Document

