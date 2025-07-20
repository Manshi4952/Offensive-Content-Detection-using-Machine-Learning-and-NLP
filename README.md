# 🛡️ Offensive Content Detection using Machine Learning and NLP

This project implements an automated system to detect offensive and hate speech in English using machine learning and NLP techniques. It classifies text into *Offensive/Hate* or *Not Offensive* categories using the new dataset called english_dataset.tsv dataset.

---

## 📌 Objectives

- Identify and flag harmful, abusive, or hate-filled content automatically.
- Assist content moderation on social media or forums in real time.

---

## 📁 Dataset

- **Name:** english_dataset.tsv
- **Source:** [english_dataset.tsv]
- **Size:** 5,852 records
- **Labels:**
  - `HOF` → Hate and Offensive
  - `NOT` → Not Offensive

---

## ⚙️ Methodology

1. **Preprocessing:**
   - Lowercasing, removing URLs/punctuation
   - Tokenization, stemming
   - Custom stopword removal (aggressive words like "bastard" and "idiot" retained)

2. **Feature Extraction:**
   - TF-IDF Vectorization (max_features = 5000)

3. **Model Training:**
   - 
   - Train/test split: 80/20

4. **Evaluation:**
   - Accuracy: ~87%
   - Precision, Recall, F1-score, Confusion Matrix

---

## 💻 Technologies Used

- Python
- Scikit-learn
- Pandas
- NLTK

---

## 🧪 Sample Prediction

```python
Input: "you are a bastard"
Output: Offensive/Hate
