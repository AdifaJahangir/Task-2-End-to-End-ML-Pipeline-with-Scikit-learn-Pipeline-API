# 📉 Customer Churn Prediction Pipeline

An end-to-end Machine Learning pipeline that predicts whether a customer is likely to churn using the **IBM Telco Customer Churn** dataset. The project demonstrates data preprocessing, feature engineering, model training, hyperparameter tuning, evaluation, and model deployment using **scikit-learn Pipelines**.

---

# 📌 Project Overview

Customer churn prediction helps businesses identify customers who are likely to leave their service. This project builds a reusable and production-ready machine learning pipeline that automates preprocessing and prediction on raw customer data.

The notebook includes:

* Data loading from a public dataset
* Data cleaning and preprocessing
* Feature encoding and scaling
* Model training
* Hyperparameter tuning
* Model evaluation
* Pipeline export using Joblib
* Prediction on new customer data

---

# 🚀 Features

* End-to-end Machine Learning workflow
* Automated preprocessing using `Pipeline`
* Feature transformation with `ColumnTransformer`
* Missing value handling
* Categorical encoding
* Numerical feature scaling
* Logistic Regression model
* Random Forest model
* Hyperparameter tuning using GridSearchCV
* Model comparison
* Pipeline serialization with Joblib
* Predicts churn from raw input data

---

# 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Joblib
* Google Colab

---

# 📂 Project Structure

```text
Customer-Churn-Pipeline/
│
├── Customer_Churn_Pipeline.ipynb
├── requirements.txt
├── README.md
├── best_pipeline.joblib
└── screenshots/
```

---

# 📊 Dataset

**Dataset:** IBM Telco Customer Churn Dataset

The dataset contains customer information such as:

* Gender
* Senior Citizen
* Partner
* Dependents
* Tenure
* Internet Service
* Contract Type
* Monthly Charges
* Total Charges
* Payment Method
* Churn Status

**Target Variable**

* Churn

  * Yes
  * No

---

# ⚙ Machine Learning Pipeline

The preprocessing pipeline performs:

* Missing value imputation
* Standard scaling of numerical features
* One-Hot Encoding of categorical features

The preprocessing is combined with the classifier into a single reusable pipeline.

---

# 🤖 Models Used

## Logistic Regression

* Binary Classification
* Fast and interpretable baseline model

## Random Forest Classifier

* Ensemble learning method
* Captures non-linear relationships
* Tuned using GridSearchCV

---

# 🔍 Hyperparameter Tuning

The project uses **GridSearchCV** to find the best model parameters.

Benefits include:

* Improved model performance
* Cross-validation
* Automatic best model selection

---

# 📈 Evaluation Metrics

The trained models are evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix

The best-performing model is selected based on evaluation metrics.

---

# 💾 Model Export

The complete fitted pipeline (preprocessing + trained model) is saved using **Joblib**.

```python
joblib.dump(best_pipeline, "best_pipeline.joblib")
```

The saved pipeline can later be loaded for prediction without repeating preprocessing steps.

---

# ▶️ Running the Project

Clone the repository

```bash
git clone https://github.com/your-username/Customer-Churn-Pipeline.git
```

Navigate to the project folder

```bash
cd Customer-Churn-Pipeline
```

Install dependencies

```bash
pip install -r requirements.txt
```

Open

```text
Customer_Churn_Pipeline.ipynb
```

Run all notebook cells sequentially.

---

# 📦 Required Libraries

* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn
* joblib

Install them using:

```bash
pip install -r requirements.txt
```

---

# 📌 Example Workflow

1. Load customer churn dataset
2. Clean the data
3. Separate features and target
4. Split into training and testing sets
5. Build preprocessing pipeline
6. Train Logistic Regression model
7. Train Random Forest model
8. Tune hyperparameters using GridSearchCV
9. Compare model performance
10. Save the best pipeline
11. Load the saved pipeline
12. Predict churn for new customers

---

# 🎯 Example Prediction

**Input**

```text
Tenure: 24
Contract: Month-to-month
Internet Service: Fiber Optic
Monthly Charges: 85.5
Payment Method: Electronic Check
```

**Output**

```text
Prediction:
Customer is likely to Churn
```

---

# 📚 Future Improvements

* XGBoost implementation
* LightGBM implementation
* Feature importance visualization
* SHAP explainability
* Flask/FastAPI deployment
* Streamlit dashboard
* Docker containerization
* Cloud deployment

---


