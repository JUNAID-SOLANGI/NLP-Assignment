# 🧠 NLP Text Classification Pipeline & Word Embedding Exploration

This repository contains an end-to-end **Natural Language Processing (NLP)** pipeline developed as part of an academic assignment. The project demonstrates core NLP skills—ranging from text cleaning and feature engineering to model training and performance evaluation—using both sparse and dense vector representations.

---

## 🔍 Use Case

**Spam Detection in SMS Messages**

The pipeline is framed around a real-world application: **telecom companies filtering spam SMS messages**.  
The stakeholder, a **telecom data team**, needs to automatically identify spam texts to improve customer trust and reduce malicious campaigns.

Dataset used: [SMS Spam Collection](https://archive.ics.uci.edu/dataset/228)

---

## 📌 Project Objectives

- Build a reproducible NLP pipeline for **text classification**.
- Compare **generative vs. discriminative** classifiers.
- Explore and evaluate both **sparse (Bag-of-Words, TF-IDF)** and **dense (Word2Vec)** text representations.
- Reflect on the performance trade-offs in terms of **accuracy, memory, and explainability**.

---


---

## 🧪 Models & Results

| Model                 | Vectorizer     | Accuracy | Precision | Recall  | F1-Score |
|----------------------|----------------|----------|-----------|---------|----------|
| Naive Bayes          | Bag-of-Words   | 0.9587   | 0.8023    | 0.9200  | 0.8571   |
| Naive Bayes          | TF-IDF         | 0.9354   | 1.0000    | 0.5200  | 0.6842   |
| Logistic Regression  | Bag-of-Words   | 0.9731   | 1.0000    | 0.8000  | 0.8889   |
| Logistic Regression  | TF-IDF         | 0.9228   | 0.9706    | 0.4400  | 0.6055   |
| Linear SVM           | Bag-of-Words   | 0.9767   | 1.0000    | 0.8267  | 0.9051   |
| Linear SVM           | TF-IDF         | 0.9713   | 1.0000    | 0.7867  | 0.8806   |

---

## 📈 Key Highlights

- **Text Preprocessing**: Lowercasing, regex cleaning, tokenization, stopword removal, lemmatization.
- **Feature Engineering**:
  - Sparse: Bag-of-Words and TF-IDF (Unigrams + Bigrams)
  - Dense: Word2Vec (Skip-Gram)
- **Models Used**:
  - Generative: Multinomial Naive Bayes
  - Discriminative: Logistic Regression, Linear SVM
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score (Macro)

---

## 📊 Analysis

- **Discriminative models** (especially Linear SVM) consistently outperform Naive Bayes in both accuracy and F1-score.
- **Bag-of-Words** outperformed TF-IDF across all classifiers—likely due to TF-IDF over-penalizing frequent spam-related terms.
- **Dense embeddings (Word2Vec)** provided additional experimentation, though final results focused on sparse features for consistency and clarity.
- **Linear SVM + BoW** showed the best overall performance in terms of both accuracy and recall.

---

<img width="985" height="590" alt="download" src="https://github.com/user-attachments/assets/33162c0a-a993-4561-a92e-0b3404d361ea" />

