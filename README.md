# project-summarization
This project fine-tunes the pretrained bert-base-uncased transformer on the arXiv dataset for abstractive summarization of scientific papers. Leveraging Hugging Face’s Trainer and TrainingArguments, it provides an efficient, scalable pipeline with BERT tokenizer for generating clear, concise summaries.
# BERT-based Summarization Model (Abstractive)

This project implements an abstractive text summarization model using the `bert-base-uncased` transformer from Hugging Face. The model is fine-tuned on a dataset containing pairs of scientific articles and their abstracts, similar to those found on arXiv. It uses the `Trainer` API for efficient training and `CrossEntropyLoss` for evaluation.
---
## 🚀 Project Features

- Preprocessing with `BertTokenizer` (with padding/truncation)
- Custom PyTorch `Dataset` class
- Fine-tuning with Hugging Face `Trainer`
- Evaluation using `CrossEntropyLoss`
- Works on CPU and GPU (CUDA)

---

## 🧠 Model Details

- **Model:** `bert-base-uncased` (pretrained)
- **Task:** Abstractive summarization
- **Input:** Scientific article
- **Target:** Human-written abstract
- **Tokenizer:** Hugging Face BERT tokenizer
- **Loss Function:** CrossEntropyLoss

---

## 🛠️ Requirements

Install dependencies using pip:

```bash
pip install torch transformers datasets
