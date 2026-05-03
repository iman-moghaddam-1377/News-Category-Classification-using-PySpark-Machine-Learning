# 📰 News Category Classification using PySpark & Machine Learning

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![PySpark](https://img.shields.io/badge/PySpark-BigData-orange.svg)
![NLP](https://img.shields.io/badge/NLP-TFIDF-yellow.svg)
![ML](https://img.shields.io/badge/MachineLearning-Classification-red.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

---

## 📌 Project Overview

This project focuses on **news classification** using **PySpark and NLP techniques**.

Given a dataset of news articles with titles and categories, the goal is to build machine learning models that can automatically classify news into predefined categories.

---

## ⚡ Tech Stack

* **PySpark (Apache Spark)** for distributed data processing
* **Spark MLlib** for machine learning
* **Python**
* **NLP Techniques**:

  * Bag of Words (BoW)
  * TF-IDF

---

## 📊 Dataset

* News dataset containing:

  * 📰 Title (text feature)
  * 🏷️ Category (label)

---

## 🧹 Preprocessing (PySpark)

* Text cleaning and normalization
* Stopword removal
* Tokenization using PySpark
* Feature preparation using Spark pipelines

---

## 🔢 Feature Engineering

### 🔹 Bag of Words (BoW)

* Convert text into numerical vectors
* Represent word frequency in each document

### 🔹 TF-IDF

* Apply weighting to emphasize important words
* Reduce impact of common but less informative terms

---

## 🌳 Models

### 1. Decision Tree Classifier

* Trained using different **maxDepth values (3 → 8)**
* Evaluated effect of tree depth on performance

---

### 2. Hyperparameter Tuning

* **MaxBins** tested with values:

  * 4, 8, 16, 32
* Evaluated impact on model accuracy

---

### 3. Random Forest Classifier

* Built using optimal `maxDepth`
* Tested different number of trees:

  * 4, 16, 64
* Evaluated trade-off between:

  * Accuracy
  * Computational cost

---

## ⏱️ Performance Analysis

* Measured training time for classification
* Compared runtime using different numbers of Spark cores
* Analyzed scalability of PySpark implementation

---

## 📊 Results

### ✅ Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score

---

### 🔍 Key Insights

* TF-IDF improves classification performance over raw BoW
* Increasing tree depth improves accuracy up to a limit (risk of overfitting)
* Random Forest significantly outperforms a single Decision Tree
* Increasing number of trees improves performance but increases computation time
* PySpark enables scalable processing for large text datasets

---


