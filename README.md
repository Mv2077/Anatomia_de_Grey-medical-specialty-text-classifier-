# 🧠 Medical Specialty Text Classifier

## 📄 Overview
This project implements a **medical specialty classification system** based on **patient descriptions** using Natural Language Processing (NLP).

Given a short textual description of a patient's symptoms, the system predicts the most likely **medical specialty**, such as Orthopedics, Cardiology, Neurology, etc.

---

## 📊 Dataset
- **Source:** Hugging Face  
  `hpe-ai/medical-cases-classification-tutorial`
- **Input:** Cleaned patient descriptions
- **Target:** Medical specialty (13 classes)

---

## 🧹 Data Preparation
- Text lowercasing  
- Special character removal  
- Stopword removal  
- Lemmatization (NLTK)  
- Label encoding  
- Class balancing to reduce bias  

---

## 🤖 Models
The project compares multiple NLP models:

- Naive Bayes  
- Logistic Regression  
- DistilBERT  
- ModernBERT  
- GPT-2 (experimental classification)

Each model is trained, saved, and evaluated independently.

---

## 📈 Evaluation
Models are evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  

A unified evaluation pipeline allows direct comparison between models.

---

## 🚀 Deployment
The best-performing model (**ModernBERT**) is deployed using **Streamlit**, allowing users to:
- Input a patient description
- Receive a predicted medical specialty
- View a confidence score

---

## 🛠️ Tech Stack
- Python  
- PyTorch  
- Hugging Face Transformers  
- Scikit-learn  
- NLTK  
- Streamlit  

---

## ⚠️ Disclaimer
This project is for **educational purposes only** and must not be used for real medical diagnosis.
