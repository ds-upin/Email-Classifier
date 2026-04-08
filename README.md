# Spam Email Classifier

This project is a **Spam Email Classifier** built using Python and scikit-learn. It applies **Natural Language Processing (NLP)** techniques and machine learning algorithms to classify emails as **spam** or **ham (not spam)**.

The dataset contains approximately **195,000 emails**, and text features are extracted using **TF-IDF Vectorization** with **5,000 features (unigrams + bigrams)**.

Two models were implemented and compared:
- Multinomial Naive Bayes
- Random Forest

The project includes **data cleaning**, **email length analysis**, and **outlier removal using IQR (Interquartile Range)** to improve model performance.

---

## 🚀 Project Highlights

- **Dataset:** ~195k labeled emails (spam and ham)
- **Problem Type:** NLP Text Classification
- **Data Cleaning:**
  - Removed null values
  - Removed duplicate emails
  - Filtered extremely short emails
  - Removed extremely long emails using IQR
- **Feature Engineering:**
  - TF-IDF Vectorizer
  - 5,000 features
  - Unigrams and Bigrams
  - English stopword removal
- **Models Implemented:**
  - Multinomial Naive Bayes
  - Random Forest Classifier
- **Evaluation Metrics:**
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
- **Deployment Ready:**
  - Model saved using joblib

---

## 📊 Results

### 1️⃣ Multinomial Naive Bayes

**Accuracy:** 0.9400

**Classification Report**

| Class    | Precision | Recall | F1-score | Support |
|----------|-----------|--------|----------|---------|
| 0 (Ham)  | 0.93 | 0.96 | 0.94 | 21,167 |
| 1 (Spam) | 0.95 | 0.92 | 0.94 | 18,638 |

**Confusion Matrix**
[[20244 923]
[1464 17174]]


**Interpretation**

- True Negatives (Ham correctly classified): 20,244
- False Positives (Ham predicted as Spam): 923
- False Negatives (Spam predicted as Ham): 1,464
- True Positives (Spam correctly classified): 17,174

---

### 2️⃣ Random Forest (Pipeline 2)

**Accuracy:** 0.9155

---

## ⚙️ Workflow

1. Data collection
2. Data cleaning
3. Email length analysis
4. Outlier removal using IQR
5. Train-test split
6. TF-IDF feature extraction
7. Model training
8. Model evaluation
9. Model export using joblib

---

## 🧠 NLP Classification Problem

This project falls under **Natural Language Processing (NLP)** because it works with **text data (emails)** and applies machine learning techniques to understand and classify human language.

### NLP Techniques Used

- Text preprocessing
- Stopword removal
- N-grams (unigrams + bigrams)
- TF-IDF vectorization
- Text classification

### Task Type

**Text Classification** – automatically categorizing emails into Spam or Ham.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- scikit-learn
- TF-IDF Vectorizer
- Multinomial Naive Bayes
- Random Forest
---

## 📦 Installation

Clone the repository:
git clone https://github.com/ds-upin/Email-Classifier.git
cd Email-Classifier

