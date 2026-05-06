# CENG 467 - Natural Language Understanding and Generation
## Take-Home Midterm Project

This repository contains the comprehensive experimental studies and implementations for the CENG 467 Take-Home Midterm. The project explores the evolution of NLP architectures from classical statistical methods to modern transformer-based models across five core tasks.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Ao9d9jIoZU8V-Ob3nqWHskoEHdah8LHe?usp=sharing)

## 📌 Project Overview
The study investigates five fundamental NLP challenges, providing a comparative analysis of modeling paradigms, design philosophies, and failure modes:

1.  [cite_start]**Representation Learning:** Sentiment Classification on the SST-2 dataset using Sparse (TF-IDF), Dense (BiLSTM), and Contextual (DistilBERT) representations. [cite: 11, 46]
2.  [cite_start]**Named Entity Recognition (NER):** Sequence labeling on CoNLL-2003 with BiLSTM-CRF and BERT-base-cased. [cite: 11, 149]
3.  [cite_start]**Text Summarization:** Comparison of Extractive (TextRank) and Abstractive (BART-large-cnn) techniques on the CNN/DailyMail dataset. [cite: 11, 226]
4.  [cite_start]**Machine Translation:** English-to-German translation evaluation using T5-Small and Helsinki-NLP MarianMT (OPUS) on the Multi30k dataset. [cite: 11, 360]
5.  [cite_start]**Language Modeling:** Probabilistic sequence modeling comparing Statistical Bigram (MLE) and Neural GPT-2 models on WikiText-2. [cite: 11, 473, 477]

## 🛠️ Tech Stack & Environment
- [cite_start]**Platform:** Google Colab [cite: 35]
- [cite_start]**Hardware:** NVIDIA T4 GPU (CUDA-enabled) [cite: 37]
- [cite_start]**Languages:** Python 3.10+ [cite: 581]
- [cite_start]**Core Libraries:** - `transformers` & `datasets` (Hugging Face) [cite: 36]
  - [cite_start]`PyTorch` (Deep Learning Framework) [cite: 36, 581]
  - [cite_start]`evaluate` (Metrics: BLEU, ROUGE, BERTScore, METEOR, ChrF) [cite: 36, 579]
  - `sumy` (TextRank Implementation)
  - [cite_start]`NLTK` (Text Preprocessing) [cite: 36]

## 📊 Key Findings
- [cite_start]**Contextual Dominance:** Pre-trained transformer models consistently outperformed classical and recurrent architectures across all tasks due to extensive linguistic knowledge acquired during pre-training. [cite: 14, 570]
- [cite_start]**Task Specialization:** Domain-specific models (e.g., MarianMT for translation) significantly outperform general-purpose models (e.g., T5-small), highlighting the importance of targeted fine-tuning. [cite: 571]
- [cite_start]**Interpretability Trade-off:** While contextual models offer superior performance, sparse representations (TF-IDF) remain highly interpretable and computationally efficient for specific tasks like sentiment analysis. [cite: 14, 576]

## 🚀 How to Run
1.  Click the **"Open In Colab"** badge at the top of this README.
2.  Ensure your Colab runtime is set to **GPU** (Runtime -> Change runtime type -> Hardware accelerator: T4 GPU).
3.  Execute the cells sequentially. [cite_start]All dependencies are handled via `!pip install` commands within the notebook. [cite: 583]
4.  [cite_start]A global seed of **42** is used for reproducibility. [cite: 13, 39, 581]

## 📝 Repository Structure
- `ceng467_midterm.ipynb`: Full implementation, experiment logs, and qualitative analyses.
- `ceng467_report.pdf`: Detailed academic report including theoretical background, results, and error analysis.

## 👤 Author
**Ceren Nur Arıkoğlu** 
[cite_start]Computer Engineering Student [cite: 1, 8]
