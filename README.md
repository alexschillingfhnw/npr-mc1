# Natural Language Processing - Mini-Challenge 1 (Retrieval Augmented Generation)

This repository contains the code and resources for Mini-Challenge 1 of the Natural Language Processing module. The project involves the development and evaluation of a Retrieval-Augmented Generation (RAG) system to support accurate and contextually relevant responses from a Large Language Model (LLM) using external knowledge sources.

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Dara](#data)
- [Installation](#installation)

## Overview

RAG is a technique that enhances the response quality of LLMs by incorporating external facts and passages that the model may not have been trained on. This system is designed to retrieve relevant text passages from a large corpus of cleantech media articles and use them to generate accurate answers to user queries.

### Key project components

- Ingestion and Preprocessing: Cleansing and chunking of text data into manageable segments.
- Embedding and Retrieval: Mapping text chunks to high-dimensional vector embeddings for similarity-based retrieval.
- Generation: Using Azure OpenAI’s GPT-4 model to generate responses based on retrieved information.
- Evaluation: Assessing the quality and relevance of responses using human-provided gold-standard answers.

### Learning Objectives

- Text Data Preparation: Ingest, clean, and chunk textual data, then generate embeddings for efficient retrieval.
- Statistical and Neural Language Models: Apply pre-trained models for conversational response generation and evaluation.
- Transformer Models: Understand and use transformer-based models for chunk embedding and answer generation.
- NLP Tools & Frameworks: Build a modular RAG pipeline including ingestion, retrieval, generation, and evaluation.
- Evaluation Methodologies: Analyze response groundedness, plausibility, and accuracy with systematic metrics.

## Project Structure

```plaintext
├── data
│   ├── raw                  # Raw data from the cleantech corpus
│   ├── processed            # Processed and cleaned data for chunking and rag system
│   └── evaluation           # Evaluation data with gold-standard answers
│   └── experiments          # csv files containing evaluation-, retrieved-, generated- and metric data for each experiment (different chunking strategy, embedding model)
├── docs                     # Documentation files
├── src                      # Source code files for the RAG-system
├── .gitignore
└── README.md
```

## Data
- **Source:** The cleantech media corpus (10'000 articles) is available on [Kaggle](https://www.kaggle.com/datasets/jannalipenkova/cleantech-media-dataset).
- **Evaluation Data:** Human-provided query-relevant text-answer triplets, used for assessing response quality.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/alexschillingfhnw/npr-mc1.git
   ```
2. **Navigate to the project directory:**
   ```bash
   cd npr-mc1
   ```
3. **Install dependencies** (if a requirements file exists):
   ```bash
   pip install -r requirements.txt
   ```
