# 📘 AI For Bharat – AWS RAG Knowledge Systems (Complete Workshop Implementation)
### *Hands-on Labs from AWS AI for Bharat Workshop | Amazon Bedrock RAG | Multi-Modal & Advanced Retrieval Techniques*

---

## 🚀 Overview
This repository contains my completed hands-on work for the **AI For Bharat – AWS Generative AI Workshop**, where I implemented multiple Retrieval Augmented Generation (RAG) architectures using **Amazon Bedrock Knowledge Bases** and supporting AWS services.

This project includes **all workshop labs**, covering:  
✔ Core RAG concepts  
✔ Accuracy optimization  
✔ Responsible AI practices  
✔ Multi-modal RAG  
✔ Structured data RAG  
✔ Graph-based RAG  
✔ Synthetic dataset creation  

This repo documents my understanding, implementation, and learnings across all modules.

---

## 🎯 Problem Statement
Large Language Models (LLMs) hallucinate when they lack access to private, real-world, or organization-specific information.  
The workshop challenge was to build **accurate, context-aware, and scalable RAG solutions** using AWS services.

### **Goals**
- Reduce hallucinations  
- Retrieve factual knowledge from documents  
- Integrate structured, graph, and multi-modal data  
- Build production-style RAG pipelines  
- Deploy using Amazon Bedrock and serverless AWS services  

---

## 💡 Solution Summary
To solve the problem, I built RAG workflows using:

### 🔹 Retrieval (vector search + hybrid search)  
### 🔹 Augmentation (relevant chunk injection)  
### 🔹 Generation (Bedrock LLM response)  

AWS managed services made it easy to ingest data, generate embeddings, and run inference with high accuracy and scalability.

---

## 🧱 Architecture Overview

```
           ┌───────────────────────────────┐
           │        User Query             │
           └───────────────────────────────┘
                         │
                         ▼
              ┌────────────────────┐
              │   API / Lambda     │
              └────────────────────┘
                         │
                         ▼
        ┌──────────────────────────────────────┐
        │ Bedrock Knowledge Base (Embeddings)  │
        └──────────────────────────────────────┘
                         │
                         ▼
            ┌──────────────────────────┐
            │ Amazon S3 Documents/Data │
            └──────────────────────────┘
                         │
                         ▼
              ┌────────────────────┐
              │ Bedrock LLM (Claude│
              │ or Llama Models)   │
              └────────────────────┘
                         │
                         ▼
           ┌───────────────────────────────┐
           │    Final RAG Response         │
           └───────────────────────────────┘
```

---

## 📂 Repository Structure (Actual)

```
AI-For-Bharat-AWS-RAG/
│
├── .gitignore
├── requirements.txt
│
├── 01-rag-concepts/                        # Core RAG building blocks
├── 02-optimizing-accuracy-retrieved-results/ # Improving precision & recall
├── 03-responsible-ai/                      # Safety, filtering, governance
├── 04-multi-modal-rag/                     # Text + Image retrieval
├── 05-structured-rag/                      # Structured data (tables, CSV, DB)
├── 06-graph-rag/                           # Graph-based retrieval
│
├── synthetic_dataset/                      # Generated dataset samples
├── utils/                                  # Helper scripts (chunking, cleaning)
│
└── README.md                               # Documentation (this file)
```

Each folder contains notebooks, code, and outputs from the AWS workshop labs.

---

## 🛠 AWS Services Used

### **Amazon Bedrock**
- LLM inference (Claude / Llama)  
- Embedding generation  
- Knowledge Base retrieval  

### **Amazon S3**
- Document storage  
- Dataset ingestion  

### **AWS Lambda**
- RAG pipeline orchestration  
- Retrieval and augmentation logic  

### **Amazon API Gateway**
- API endpoint for client interaction  

### **IAM**
- Secure service-level permissions  

### **Optional**
- OpenSearch Serverless (Vector DB)  
- RDS / DynamoDB (Structured RAG)  

---

## ⚙️ Implementation Breakdown

### **📌 Module 01 – RAG Concepts**
- Creating a Bedrock Knowledge Base  
- Ingesting data from S3  
- Running Retrieve and Generate API  
- Running Hybrid Search (semantic + keyword)

### **📌 Module 02 – Accuracy Optimization**
- Reranking retrieved results  
- Text chunk size tuning  
- Metadata-based enrichment  
- Search scoring strategies  

### **📌 Module 03 – Responsible AI**
- Toxicity filters  
- Content moderation  
- Safe generation controls  
- Bedrock Guardrails  

### **📌 Module 04 – Multi-Modal RAG**
- Extracting embeddings from images  
- Combining text & image retrieval  
- RAG pipeline for multimodal Q&A  

### **📌 Module 05 – Structured RAG**
- Retrieving from CSV / SQL tables  
- Converting structured data to embeddings  
- Query → SQL generation → Retrieval → LLM reasoning  

### **📌 Module 06 – Graph RAG**
- Building entity graphs  
- Relationship-aware retrieval  
- Graph-based context augmentation  

---

## 📸 Workshop Completion Screenshots
All screenshots of lab executions are included in the folder:

```
/workshop-screenshots/
```

These include:
- Bedrock Knowledge Base setup  
- Retrieval API responses  
- Multi-model RAG outputs  
- Graph RAG output  
- Successful lab completion screens  

---

## 📘 Key Learnings
Through this workshop, I learned:

✨ How enterprise RAG systems work end-to-end  
✨ Importance of chunking, embedding models, and retrieval tuning  
✨ Multi-modal RAG for images + text  
✨ Graph-aware retrieval for complex reasoning  
✨ Responsible and safe AI practices on AWS  
✨ Serverless architecture for scalable AI applications  

---

## 🔗 References
- AWS Bedrock Documentation  
- OpenSearch Vector Search Docs  
- AI for Bharat Workshop Materials  

---

## 🧑‍💻 Author
**Aryan Vishal Jalak**  


