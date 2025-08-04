# 💳 Credit Card Fraud Detection – KNIME Project

## 🧾 Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning workflows in **KNIME Analytics Platform**. Due to the high class imbalance in fraud datasets, the project includes advanced techniques like **SMOTE** for oversampling and ensemble models like **Random Forest** and **Isolation Forest** to improve accuracy and robustness. The objective is to build an efficient, scalable fraud detection pipeline using a no-code/low-code approach.


## 📁 Dataset

- **Source:** [Kaggle – Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)  
- **Size:** 284,807 transactions, 492 fraud cases  
- **Features:** 30 anonymized features (V1 to V28), `Amount`, and `Class` (0 = Legit, 1 = Fraud)


## ⚙️ Tools & Technologies

- **Platform:** KNIME Analytics Platform  
- **Algorithms Used:**  
  - Random Forest  
  - Isolation Forest  
  - SMOTE (Synthetic Minority Oversampling Technique)  
- **Nodes:** Data Reader, Data Preprocessing, Partitioning, SMOTE, Scorer, Model Training, Confusion Matrix


## 🔍 Workflow Steps

1. **Data Import & Cleaning**
   - Loaded dataset using CSV Reader node
   - Handled missing values and performed normalization

2. **Data Balancing**
   - Applied **SMOTE** to oversample minority (fraud) class

3. **Model Training**
   - Trained multiple models including **Random Forest** and **Isolation Forest**
   - Tuned hyperparameters using **Parameter Optimization Loop**

4. **Model Evaluation**
   - Evaluated using confusion matrix, precision, recall, F1-score
   - Compared performance across models for fraud detection accuracy

5. **Visualization**
   - Used Box Plot, ROC Curve, and Score Distributions to interpret model behavior


## 📊 Results

| Model           | Accuracy | Precision | Recall | F1-Score |
|----------------|----------|-----------|--------|----------|
| Random Forest   | ~99.3%   | 87%       | 82%    | 84%      |
| Isolation Forest| ~95%     | 73%       | 68%    | 70%      |

> ✅ **Random Forest with SMOTE** gave the best results in detecting fraud transactions.


## 📸 Sample Workflow Screenshot

*(Insert a screenshot of your KNIME workflow here)*


## 🚀 How to Run

1. Download and install [KNIME Analytics Platform](https://www.knime.com/downloads).
2. Clone this repository or download the `.knwf` workflow file.
3. Open the workflow in KNIME and execute all nodes from start to finish.
4. View results and visualizations in output nodes.


## 📌 Future Enhancements

- Integrate real-time detection using streaming data  
- Deploy model using KNIME Server or REST API  
- Compare with deep learning models using Python integration

