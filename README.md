
# **Sentiment Analysis of Google Play Store Reviews**

## **Project Overview**
This project uses Natural Language Processing (NLP) to classify Google Play Store app reviews into **Positive**, **Neutral**, and **Negative** sentiments. It analyzes real user feedback to understand satisfaction drivers and identify areas for app improvement.

---

## **Dataset**
- **Source:** Kaggle – Google Play Store Reviews Dataset
- **Records:** ~12,000 app reviews with ratings and review text
- **Features:**
  - `review`: Text of user review
  - `rating`: Star rating (1–5)
  - `Sentiment`: Labeled sentiment (derived from rating)

---

## **Steps Implemented**
1. **Exploratory Data Analysis (EDA)**  
   - Visualized sentiment distribution, review length, and ratings across sentiments.
2. **Preprocessing**  
   - Cleaned text: lowercasing, punctuation removal, and stopword filtering.
   - Encoded sentiments and vectorized reviews using **TF-IDF**.
3. **Model Building**  
   - Trained **Logistic Regression**, **Naive Bayes**, and **Random Forest**.
   - Best model: Logistic Regression with **accuracy ≈ 90%**.
4. **Explainability**  
   - Applied **LIME** to identify words driving predictions.
   - Positive cues: *“love”*, *“easy”*, *“helpful”*.
   - Negative cues: *“crash”*, *“ads”*, *“buggy”*.
5. **Insights**  
   - Most dissatisfaction is due to performance issues and excessive ads.
   - Improving app speed and reducing bugs can boost user satisfaction.

---

## **Results**
- **Best Model:** Logistic Regression  
- **Accuracy:** ~90%, with balanced precision and recall across classes.

---

## **Next Steps**
- Build a **Streamlit dashboard** for real-time sentiment visualization.
- Incorporate topic modeling (LDA) to group complaints and feature requests.

---
