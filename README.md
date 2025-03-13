# 🔍 Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset used contains real transactions made by European cardholders in September 2013. Due to confidentiality, the features are anonymized except for `Time` and `Amount`.

---

## 📌 **Project Overview**
- **Problem Statement:** Detect fraudulent transactions in a dataset of credit card transactions.
- **Tech Stack:** Python, Jupyter Notebook, Scikit-Learn, Pandas, Matplotlib, Seaborn
- **Dataset:** [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

## 📂 **Project Files**
- `credit_card_fraud_detection.ipynb` → Jupyter Notebook with data analysis, preprocessing, and model training.
- `requirements.txt` → List of required dependencies.
- `README.md` → Project documentation.

---

## 🛠 **Installation & Setup**
1. **Clone this repository**:
   ```bash
   git clone https://github.com/YourUsername/credit-card-fraud-detection.git
   cd credit-card-fraud-detection

📊 Dataset Details
The dataset contains 284,807 transactions with 492 fraudulent cases (0.172% of the data).
Features V1 to V28 are anonymized.
Time represents seconds elapsed between transactions.
Amount is the transaction amount.
Class:
0 → Legitimate transaction
1 → Fraudulent transaction

🔬 Data Preprocessing
Handling Imbalance: Used SMOTE (Synthetic Minority Over-sampling Technique) to balance fraud cases.
Feature Scaling: Applied StandardScaler to normalize Amount and Time.
Splitting Data: Used 80-20 train-test split.

🤖 Machine Learning Models
The following models were trained and evaluated:

Logistic Regression
Random Forest Classifier
XGBoost Classifier
Support Vector Machine (SVM)
Neural Networks (MLPClassifier)
Evaluation Metrics Used:

Accuracy
Precision, Recall & F1-score
ROC-AUC Score
Confusion Matrix

📈 Results & Insights
Random Forest & XGBoost performed best with an AUC-ROC score of ~99%.
Precision-Recall Tradeoff: Due to class imbalance, Recall is prioritized over Precision.
SMOTE Improved Recall: Balancing the dataset helped in detecting more fraudulent cases.
