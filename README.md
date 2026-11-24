# Intelligent Anomaly Detection Using Machine Learning

## 📌 Project Overview
This project focuses on detecting anomalous patterns (fraud) in credit card transactions. The Kaggle dataset contains 284,807 transactions, with only 0.172% being fraudulent (highly imbalanced). The goal was to build a model that can accurately distinguish normal from anomalous observations.

## 🛠️ Data Preprocessing & Feature Engineering
- **Data Cleaning:** Verified zero missing values and checked dataset dimensions.
- **Feature Scaling:** Standardized `Amount` and `Time` features using `StandardScaler`.
- **Feature Engineering:** Extracted the `Hour` from the `Time` column to help the model detect late-night fraudulent behavior.
- **Handling Imbalance:** Applied **SMOTE** (Synthetic Minority Over-sampling Technique) on the training set to balance the fraud and normal classes.

## 🤖 Model & Evaluation
- **Algorithm:** Random Forest Classifier.
- **Metrics:** Evaluated using Precision, Recall, F1-Score, and Confusion Matrix.
- **Results:** Achieved an **F1-score of 0.88** for the fraud class, successfully catching 87% of the fraudulent transactions.

## 📂 Files in this Repository
- `Untitled1.ipynb`: The complete Google Colab notebook with data loading, preprocessing, feature engineering, SMOTE, model training, and evaluation.

## 🚀 How to Run
1. Open the `.ipynb` file in Google Colab.
2. Upload the `creditcard.csv` dataset to your Colab environment.
3. Run all cells to see the preprocessing and model results.
