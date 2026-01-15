# Fake News Detection using Semantic Classification 📰🛡️

> **An AI-powered solution to distinguish between credible news and misinformation using Word2Vec semantic embeddings and Random Forest.**

## **Project Overview**
In an era of viral misinformation, keyword-based detection is no longer enough. This project moves beyond simple "syntax" and uses **Semantic Classification** to understand the actual meaning of news articles. By leveraging NLP techniques, the model identifies the tone and context used in True vs. Fake reporting.

## **Problem Statement**
The goal is to develop a supervised model that categorizes news based on its semantic relations. This addresses the business need for real-time, automated verification systems for digital news platforms.



## **Project Pipeline**
1. **Text Preprocessing:** Cleaned text via Lemmatization and POS filtering to retain meaningful nouns.
2. **Exploratory Data Analysis (EDA):** Analyzed character lengths and N-gram frequencies to identify linguistic "fingerprints" of fake news.
3. **Semantic Embedding:** Utilized **Word2Vec (Google News 300)** to convert text into mathematical vector representations.
4. **Model Building:** Compared Logistic Regression and Decision Trees against a **Tuned Random Forest**.

## **Results & Insights**
* **Best Model:** Random Forest Classifier.
* **Key Finding:** True news leans toward institutional/factual language (Government, Official), while Fake news utilizes sensationalist/engagement terms (Video, Shocking, Conspiracy).
* **Metric:** Prioritized **F1-Score** to balance Precision and Recall, ensuring credible news isn't accidentally flagged.



## **📂 Repository Structure**
* [**data/**](./data/): Raw news dataset.
* [**docs/**](./docs/): Project presentation and theoretical Q&A.
* [**notebooks/**](./notebooks/): End-to-end Python implementation.

## **Conclusions**
The implementation of semantic features allowed the model to achieve high performance with minimal overfitting. This approach demonstrates that understanding "context" is the key to scaling truth in digital media.
