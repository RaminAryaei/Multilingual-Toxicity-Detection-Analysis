# Phase 1: Benchmarking Transformer Architectures for Toxicity Detection 📊

This directory contains the initial benchmarking of state-of-the-art Transformer models for classifying toxic comments. The goal was to establish a baseline performance before moving towards multilingual and xLSTM-based architectures.

## 🎯 Objectives
- Implement and fine-tune **BERT-Base**, **RoBERTa-Base**, and **DistilBERT**.
- Compare performance using standard NLP metrics (Accuracy, F1-Score, Precision, and Recall).
- Analyze the trade-off between model accuracy and computational efficiency.

## 🛠️ Experimental Setup
- **Dataset:** Jigsaw Toxic Comment Classification (sampled for benchmarking).
- **Tooling:** Python, Hugging Face Transformers, PyTorch.
- **Hardware:** Google Colab T4 GPU.
- **Data Acquisition:** Accessed via Kaggle API.

## 📈 Performance Results
Based on our experiments, the models performed as follows:

| Model Architecture | Accuracy | F1-Score | Precision | Recall |
| :--- | :---: | :---: | :---: | :---: |
| **RoBERTa-Base** | **0.96** | **0.92** | **0.93** | **0.91** |
| BERT-Base | 0.95 | 0.90 | 0.91 | 0.89 |
| DistilBERT | 0.94 | 0.88 | 0.89 | 0.87 |

## 💡 Key Findings
1. **RoBERTa-Base** proved to be the most robust model, achieving the highest scores across all metrics.
2. **BERT-Base** provided a very stable and reliable baseline.
3. **DistilBERT**, while slightly less accurate, was significantly faster, making it ideal for large-scale real-time inference.

---
*This research is conducted under the supervision of **Dr. Maryam Rahmaninia**.*
