# Source Code

This folder contains all the core notebooks used for data preprocessing, analysis, chunking, embedding generation, RAG pipeline creation and evaluation.

### **`playground`**
- A workspace for experimenting with data preprocessing techniques such as regex, structural analysis, and cleaning methods.

---

## Notebooks Overview

### **`01_data-preprocessing.ipynb`**
- Cleans and preprocesses raw Cleantech data.
- Handles formatting, removing noise and preparing the data for downstream tasks.

### **`02_data-analysis.ipynb`**
- Analyzes the preprocessed data to understand its structure, quality and distribution.
- Generates visualizations and statistics for insights.
- Helps us make decisions for the next tasks

### **`03_chunking-and-embeddings.ipynb`**
- Implements text chunking strategies and embedding generation using various models.
- Prepares data for retrieval in the RAG pipeline.

### **`04_rag-chain.ipynb`**
- Builds the RAG pipeline with vector storage, retrieval, reranking, answer generation.
- Integrates embedding-based retrieval and generation for answering queries.

### **`05_evaluation.ipynb`**
- Evaluates the performance of the RAG pipeline.
- Includes intrinsic (BLEU, ROUGE, cosine similarity) and extrinsic (LLM-based) evaluation metrics.
- Supports both automated and manual evaluation.
