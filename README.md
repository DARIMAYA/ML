# Machine Learning Projects

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python">
  <img src="https://img.shields.io/badge/Machine%20Learning-NLP%20%7C%20CV-green">
  <img src="https://img.shields.io/badge/Status-Active-success">
  <img src="https://img.shields.io/badge/Focus-Research%20%26%20Practice-orange">
</p>

## About

This repository contains a collection of machine learning projects focused on:

- **Natural Language Processing (NLP)**
- **User behavior analysis**
- **Clustering & feature engineering**
- **Computer Vision**
- **Classification tasks**

The projects explore real-world data scenarios, combining statistical methods with modern ML approaches.

---

## Repository Structure
```txt
ML/
├── author_style/
│   ├── data/
│   ├── features/
│   └── model.py
├── som_text_analysis/
│   ├── som.py
│   └── utils.py
├── commenters_clustering/
│   ├── clustering.ipynb
│   └── troll_score.py
├── keywords_analysis/
│   └── tfidf_analysis.py
├── grain_classifier/
│   ├── train.py
│   └── resnet_model.py
└── phishing_detection/
    ├── data/
    └── classifier.py
```

---

## Projects Overview

### Author Style Detection

> Analysis of textual features to identify and model author-specific writing style.

- Extracted linguistic features
- Style modeling and comparison

---

### Text Analysis & SOM Clustering

Extraction of simple but expressive linguistic features:

- vowels count
- punctuation patterns (`. ! ?`)

Clustering is performed using:

- **Self-Organizing Maps (Kohonen Network)**

---

### Commenters Clustering & Behavior Analysis

Clustering users based on communication style.

**Features:**
- text length
- emotional punctuation
- uppercase ratio
- lexical diversity
- speech markers

**Extended analysis:**
- toxicity
- political & conspiracy vocabulary
- politeness markers

**Methods:**
- K-Means
- PCA (visualization)
- TF-IDF + cosine similarity

**Additional metric:**
- `troll_score` — detects potentially toxic or conflict-driven users

---

### Keywords & Topic Relevance Analysis

- Keyword extraction using **TF-IDF**
- Matching article vocabulary with comments

**Metrics:**
- keyword frequency
- topic relevance (%)
- per-user statistics

Helps distinguish:
- meaningful discussion
- off-topic comments

---

### Grain Image Classification (ResNet50)

Image classification using transfer learning.

| Component | Description |
|-----------|-------------|
| **Model** | ResNet50 |
| **Backbone** | frozen convolutional base |
| **Head** | trained classification head |

**Data structure:**
train/
test/
format.json
**Output:** CSV with predictions
- image path
- true label
- predicted label

---

### Phishing Email Detection

Binary classification:

- legitimate emails
- phishing emails

**Dataset:** `email_phishing_data.csv`

**Features include:**
- word statistics
- links & domains
- email addresses
- spelling errors
- urgency keywords

---

## Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-black?logo=python">
  <img src="https://img.shields.io/badge/Scikit--Learn-orange?logo=scikitlearn">
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow">
  <img src="https://img.shields.io/badge/PyTorch-red?logo=pytorch">
</p>

| Area | Technologies |
|------|--------------|
| **Machine Learning** | Scikit-learn, TensorFlow, PyTorch |
| **NLP** | TF-IDF, cosine similarity |
| **Clustering** | K-Means, Self-Organizing Maps (SOM) |
| **Dimensionality Reduction** | PCA |
| **Computer Vision** | ResNet50, transfer learning |

---

## Quick Start

```bash
git clone https://github.com/DARIMAYA/ML.git
cd ml-projects
pip install -r requirements.txt
