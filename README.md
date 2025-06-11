# 📰 Fake News Detection using Semantic Classification

This project aims to detect and classify fake news articles using semantic text analysis and machine learning. By leveraging **Word2Vec embeddings** and supervised learning models, the system identifies recurring linguistic patterns that help distinguish between genuine and fake news articles.

---

## 📌 Objective

- Build a semantic classification model using **Word2Vec** and supervised learning techniques.
- Classify news articles as either *true* or *fake* based on their textual meaning, not just syntax.

---

## 🧠 Methodology (CRISP-DM Framework)

1. **Business Understanding** – Address the challenge of fake news and its impact on public trust.
2. **Data Understanding** – Explore `True.csv` and `Fake.csv` datasets (21k and 23k samples respectively).
3. **Data Preparation** – Clean and merge data, apply POS-based lemmatization, remove punctuation/digits.
4. **Feature Engineering** – Generate semantic vectors using a pre-trained **Word2Vec (GoogleNews-300)** model.
5. **Model Building** – Train and evaluate:
   - Logistic Regression
   - Decision Tree
   - Random Forest
6. **Evaluation** – Compare models based on Accuracy, Precision, Recall, and F1-Score.

---

## 🛠️ Techniques & Tools Used

- **Language**: Python
- **Libraries**: pandas, numpy, spaCy, gensim, matplotlib, seaborn, scikit-learn
- **Embedding**: Word2Vec (`GoogleNews-vectors-negative300.bin`)
- **Environment**: Jupyter Notebook, Google Colab
- **Storage**: Google Drive for data/model integration

---

## 📊 Model Performance

| Model              | Train Accuracy | Validation Accuracy | Validation Recall |
|-------------------|----------------|----------------------|--------------------|
| Logistic Regression | 86.6%          | 84.0%                | **90.5%**          |
| Decision Tree      | 99.7%          | 74.2%                | 68.9%              |
| Random Forest      | 90.4%          | 77.7%                | 75.7%              |

> ✅ **Logistic Regression** was the top performer and recommended for deployment.

---

## 🔍 Key Insights

- Fake news often includes emotionally charged or speculative language.
- Word2Vec helped extract meaningful semantic patterns beyond surface-level word matching.
- Logistic Regression generalized well and achieved high recall, minimizing false negatives.

---

## ✅ Recommendations

- Use Logistic Regression for production-level screening.
- Explore transformer-based models (e.g., BERT) for improved contextual understanding.
- Regularly retrain the model to keep up with evolving misinformation patterns.

---

## 👨‍💻 Author

**Deebesh S,** **Rahul Shetty,** **Rahul Singh**  
*Data Science | Machine Learning | NLP Enthusiast*
