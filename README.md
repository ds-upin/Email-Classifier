# Spam Email Classifier

This project is a **spam email classifier** built using Python and scikit-learn. It uses a **Multinomial Naive Bayes** model trained on **195,000 emails** with **5,000 TF-IDF features** to classify emails as spam or ham (not spam).

---

## 🚀 Project Highlights

- **Dataset:** 190k emails (spam and ham)  
- **Features:** 5,000 TF-IDF features (unigrams + bigrams)  
- **Model:** Multinomial Naive Bayes  
- **Performance:** High accuracy on unseen emails  
- **Deployment:** Model saved using `joblib` for reuse

---

## 📊 Results

**Accuracy:** 0.9400

**Classification Report:**

| Class    | Precision | Recall | F1-score | Support |
|----------|-----------|--------|----------|---------|
| 0 (Ham)  |   0.93    |  0.96  |   0.94   |  21167  |
| 1 (Spam) |   0.95    |  0.92  |   0.94   |  18638  |

**Confusion Matrix:**
[[ 20244    923 ]
[  1464   17174]]



- **True Negatives (Ham correctly classified):** 20,244  
- **False Positives (Ham misclassified as Spam):** 923  
- **False Negatives (Spam misclassified as Ham):** 1,464  
- **True Positives (Spam correctly classified):** 17,174  

---

## 💡 Key Learnings

- Even simple models like **Multinomial Naive Bayes** can achieve **high accuracy** with appropriate feature extraction.  
- TF-IDF vectorization of text captures both keywords and important patterns.  
- Real-world validation on Gmail emails ensures practical applicability.  

---
