# Comment Category Prediction using NLP and Machine Learning

## Overview

This project focuses on automatically classifying user comments into predefined categories using Natural Language Processing (NLP) and Machine Learning techniques.

The objective is to build a robust multi-class classification model capable of identifying comment categories based on textual content and auxiliary numerical features.

The project was completed as part of the IIT Madras BS Degree Program in Data Science and Applications.

---

## Problem Statement

Online platforms receive large volumes of user-generated content every day. Manual moderation and categorization of comments is time-consuming and difficult to scale.

The goal of this project is to develop a machine learning pipeline that can automatically predict the category of a comment using both text and metadata features.

---

## Dataset

The dataset contains:

* User comments (text data)
* Numerical features such as upvotes, downvotes, and additional indicators
* Target labels representing comment categories

The training dataset contains approximately 198,000 records, while the test dataset contains approximately 102,000 records.

---

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

* Dataset inspection using `.info()` and `.describe()`
* Missing value analysis
* Duplicate detection
* Class distribution analysis
* Numerical feature exploration
* Text length and word count analysis
* Temporal feature analysis

### 2. Data Preprocessing

* Missing comment values replaced with empty strings
* High-missing-value columns analyzed and excluded from baseline modeling
* Train-validation split
* Feature scaling using StandardScaler

### 3. Feature Engineering

#### Text Features

* Character Count
* Word Count
* Capital Letter Count
* Exclamation Count
* Question Mark Count

#### Temporal Features

* Hour
* Day of Week
* Month

#### NLP Features

* TF-IDF Vectorization
* Unigrams, Bigrams, and Trigram experiments

---

## Models Evaluated

The following machine learning models were trained and compared:

* Logistic Regression
* SGD Classifier
* Multinomial Naive Bayes
* Linear Support Vector Machine (Linear SVC)
* K-Nearest Neighbors (KNN)
* Bagging Methods
* Boosting Methods
* Multi-Layer Perceptron (MLP)

Additional experiments were conducted using:

* Hyperparameter Tuning
* Dimensionality Reduction (Truncated SVD)
* Feature Selection
* Class Weight Balancing

---

## Hyperparameter Tuning

Model performance was improved through systematic experimentation with:

### Logistic Regression

* Different values of regularization parameter (C)

### SGD Classifier

* Different values of alpha

The best-performing configuration was selected based on validation performance.

---

## Model Evaluation

Models were evaluated using:

* Precision
* Recall
* F1 Score
* Macro F1 Score
* Classification Report

The final model was chosen after comparing multiple algorithms and tuning strategies.

---

## Final Model

The best-performing solution consisted of:

* TF-IDF Vectorization
* Numerical Feature Scaling
* Logistic Regression
* Class Weight Balancing

This combination provided the best balance between performance, interpretability, and computational efficiency.

---

## Additional Experiments

After obtaining a competitive submission, further experiments were performed to explore possible improvements:

* Alternative Logistic Regression configurations
* Different TF-IDF settings
* Additional feature engineering
* Identity-based features
* Text signal analysis
* Temporal feature enhancements

These experiments were conducted to better understand model behavior and identify potential future improvements.

---

## Key Learnings

Through this project, I learned:

* End-to-end machine learning workflow
* Exploratory Data Analysis (EDA)
* Text preprocessing for NLP tasks
* TF-IDF vectorization
* Feature engineering and selection
* Hyperparameter tuning
* Model evaluation and comparison
* Handling class imbalance
* Dimensionality reduction techniques
* Practical machine learning experimentation

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* SciPy

### Development Environment

* Jupyter Notebook
* Google Colab


---

## Author

**Sana Ilahi**

BS in Data Science and Applications — IIT Madras

M.Sc. Artificial Intelligence & Machine Learning — Jamia Millia Islamia
