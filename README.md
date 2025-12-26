#  Breast Cancer Classification using Machine Learning

##  Project Overview
In this HealthTech project, I built a machine learning model to predict whether a breast tumor is **Malignant (Cancerous)** or **Benign (Non-cancerous)** based on digital image features. 

The goal was not just high accuracy, but **high sensitivity (Recall)**—minimizing "False Negatives" to ensure no cancer cases are missed during diagnosis.

##  Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
* **Dataset:** [Breast Cancer Wisconsin (Diagnostic) Data Set](https://archive.ics.uci.edu/ml/datasets/breast+cancer+wisconsin+(diagnostic))

##  Key Steps
1.  **Data Extraction:** Loaded data directly from the UCI Machine Learning Repository.
2.  **Exploratory Data Analysis (EDA):** Analyzed feature correlations and distributions; identified high multicollinearity among geometric features (Radius, Area, Perimeter).
3.  **Feature Engineering:** Removed highly correlated features (>0.9) to reduce redundancy and scaled data using `StandardScaler`.
4.  **Model Comparison:** * *Logistic Regression* (Baseline)
    * *Random Forest Classifier* (Ensemble)

##  Results
Surprisingly, the simpler **Logistic Regression** model outperformed the Random Forest model for this specific dataset.

* **Accuracy:** 97.37%
* **Recall (Malignant):** 93% (High sensitivity to cancer detection)
* **Precision (Malignant):** 100% (Zero False Positives)

##  Medical Insight
Through feature importance analysis, I found that **Concave Points**, **Area**, and **Texture** were the strongest predictors of malignancy. The project prioritized **Recall** because in a medical setting, missing a cancer diagnosis (False Negative) is the most critical error to avoid.

##  How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/YourUsername/breast-cancer-classification.git](https://github.com/YourUsername/breast-cancer-classification.git)
