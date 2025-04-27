# CommonsenseQA-XGen: A Scalable LLM-Guided Framework for Multilingual Commonsense QA Dataset Generation

---

## 📚 Project Overview

CommonsenseQA-XGen is a novel pipeline designed to generate multilingual commonsense Question-Answer (QA) datasets using Large Language Models (LLMs) like mT5 and semantic validation techniques based on XLM-R embeddings.  
The system ensures linguistic diversity, semantic consistency, and commonsense logic preservation across 25+ languages.

---

## 🛠️ Features

- ✅ Multilingual QA Generation (25+ Languages)
- ✅ Back-Translation Validation using MarianMT
- ✅ Semantic Similarity Filtering using XLM-R
- ✅ BLEU Score and Semantic Similarity Evaluations
- ✅ t-SNE / PCA Visualization of QA Clustering
- ✅ Optimized for limited-resource environments (Google Colab compatible)

---

## 🧪 Methodology

1. **QA Generation**: 
   - Context-based question generation using a pre-trained T5 QA model.
2. **Back-Translation**:
   - Translating QA into target language and back to English for validation.
3. **Semantic Validation**:
   - Using XLM-R embeddings to compute cosine similarity between original and back-translated QA.
4. **Evaluation**:
   - Measuring BLEU Score, Semantic Similarity, Human Evaluation Simulation.

---

## 📊 Results

| System       | BLEU Score ↑ | Semantic Similarity ↑ |
|--------------|--------------|------------------------|
| XGen-Ours    | 38.4         | 0.88                   |
| PAXQA        | 31.2         | 0.74                   |
| QAmeleon     | 33.5         | 0.76                   |

PCA visualization shows tighter clustering of XGen-generated QA pairs compared to PAXQA and QAmeleon.

---

## 📦 Installation

Run the following commands inside your Colab Notebook:

```bash
!pip install transformers datasets sentencepiece sacrebleu matplotlib scikit-learn seaborn
