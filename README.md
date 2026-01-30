# Sentiment Analysis: VADER vs. RoBERTa 📊🤖

This project explores automated sentiment analysis on product reviews using two distinct approaches: a traditional Lexicon-based method (**VADER**) and a Deep Learning Transformer model (**RoBERTa**). The analysis is performed on the **Amazon Fine Food Reviews** dataset.


## 🙏 Credits & Attribution
This project was developed by following the tutorial by Rob Mulla.
Tutorial Video: [Python Sentiment Analysis Project with VADER and RoBERTa](https://youtu.be/QpzMWQvxXWk)
Rob Mulla's Channel: [link](https://www.youtube.com/@robmulla) 

## 📖 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Methods](#methods)
- [Results](#results)
- [Installation & Usage](#installation--usage)

## ✨ Overview
The goal of this project is to compare how a "Bag of Words" approach (VADER) handles sentiment versus a context-aware model (RoBERTa). 

**Key Steps:**
1.  **Exploratory Data Analysis (EDA):** Visualizing review score distributions using Matplotlib and Seaborn.
2.  **Basic NLP:** Utilizing NLTK for tokenization, POS tagging, and Named Entity Recognition (NER).
3.  **VADER Analysis:** Scoring reviews as Positive, Negative, or Neutral based on word intensity.
4.  **RoBERTa Model:** Leveraging a pre-trained Transformer model from the Hugging Face Hub (`cardiffnlp/twitter-roberta-base-sentiment`) to capture complex linguistic nuances.

## 📂 Dataset
The project uses the **Amazon Fine Food Reviews** dataset from Kaggle. For computational efficiency and demonstration purposes, the analysis was performed on a sampled subset of 500 reviews.

## 🛠 Methods

### 1. VADER (Valence Aware Dictionary and sEntiment Reasoner)
VADER uses a "Bag of Words" approach where each word is scored and combined to provide a total polarity score. 
* **Pros:** Fast; no training required; works well on social media/review text.
* **Cons:** Struggles with sarcasm and complex sentence structures as it ignores word context.

### 2. RoBERTa Pre-trained Model
This model is a context-aware Transformer. Unlike VADER, it accounts for the relationship between words in a sentence, allowing it to understand more complex sentiments.
* **Pros:** Highly accurate; understands context and linguistic nuances.
* **Cons:** Computationally more intensive than Lexicon methods.

## 📈 Results
The analysis includes visualizations comparing the `compound` sentiment scores against the actual Amazon Star Ratings, demonstrating the strengths and limitations of both models when compared to human-labeled data.

## 🚀 Installation & Usage
To run the notebook, ensure you have the following libraries installed:
Choose a platform of your choice: e.g. Kaggle, VS Code, ...

```bash
pip install pandas numpy matplotlib seaborn nltk transformers scipy tqdm
```

