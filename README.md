# 🧠 Medical Specialty Text Classifier

##How to run
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1KEkmrANIn5rIWcg7N5m-9jTzYsWEW7OQ)

## 📄 Overview
This project implements a **medical specialty classification system** using Natural Language Processing (NLP).

Given a **patient description** (not a full medical transcription), the system predicts the most likely **medical specialty** such as Orthopedics, Cardiology, Neurology, Psychiatry, etc.

---

## 📊 Dataset
- **Source:** Hugging Face  
  `hpe-ai/medical-cases-classification-tutorial`
- **Input:** Cleaned patient descriptions
- **Output:** Medical specialty (13 classes)

---

## 🧹 Data Preparation
- Lowercasing  
- Special character removal  
- Stopword removal  
- Lemmatization (NLTK)  
- Label encoding  
- Class balancing  

---

## 🤖 Models
The project compares several models:

- Naive Bayes  
- Logistic Regression  
- DistilBERT  
- ModernBERT  
- GPT-2 (experimental)

Each model is trained and evaluated independently.

---

## 📈 Evaluation
Models are evaluated using:
- Precision  
- Recall  
- F1-score  

A unified evaluation pipeline enables fair comparison across models.

---

## 🚀 Deployment
The best-performing model (**ModernBERT**) is deployed using **Streamlit**, allowing users to:
- Input a patient description
- Receive the predicted medical specialty
- View a confidence score

---

## 🛠️ Tech Stack
Python · PyTorch · Hugging Face · Scikit-learn · NLTK · Streamlit

---

## ⚠️ Disclaimer
This project is for **educational purposes only** and must not be used for real medical diagnosis.
