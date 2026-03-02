# assignment_6_aig230
**Student:** Pratham Shrestha  


In this assingment 

This repository contains my implementation for Lab 6 of AIG230, focused on classical and neural language modeling.

---

## 📂 Repository Structure

```text
AIG230_Lab6_PRATHAM_SHRESTHA/
│
├── assignment_6_aiq230/
│   ├── start_code/
│   └── assignment_part_B_starter.ipynb  # Neural Language Model (Part B)
│
├── assignment_partA.ipynb               # N-gram Language Model (Part A)
├── .gitignore
└── README.md

# Part A – N-gram Language Model

## Overview

In Part A, I implemented a trigram language model with smoothing(Lidstone smoothing with k = 0.001).

### Key Steps

- Sentence-level data split (80% train, 10% validation, 10% test)
- Vocabulary built from **training split only**
- Rare words mapped to `<unk>` using `min_freq`
- Trigram model trained using:
  - Lidstone smoothing

### Reported Metrics

- Number of sentences per split
- Number of tokens per split
- Vocabulary size (train only)
- Validation perplexity
- Final test perplexity
- 3 generated text samples (30+ tokens each)

---

# Part B – Neural Language Model

## Overview

In Part B, I implemented a neural language model using PyTorch.

### Model Architecture

- Embedding layer
- Hidden layers
- Linear output layer
- CrossEntropyLoss
- Optimizer (Adam)

### Training

- Trained for multiple epochs
- Training loss tracked per epoch
- Validation perplexity computed per epoch
- Final test perplexity reported

### Outputs Included

- Training loss plot
- Validation perplexity per epoch
- Final test perplexity
- 3 generated samples (30+ tokens each)
- Brief qualitative analysis of generated text

---

# 📊 Evaluation Metric

Perplexity is used to evaluate model performance.
Lower perplexity indicates better predictive performance.

---

# ⚙️ Requirements

- Python 3.x
- PyTorch
- NLTK
- Matplotlib
- NumPy

Install dependencies:

```bash
pip install torch nltk matplotlib numpy