# Breast Cancer Classification with GridSearchCV

## 📌 Project Overview

This project demonstrates Machine Learning model training and
hyperparameter tuning using Random Forest on the Breast Cancer dataset.

------------------------------------------------------------------------

## 📂 Dataset

-   File: breast-cancer.csv
-   Target Column: diagnosis
-   Problem Type: Binary Classification

------------------------------------------------------------------------

## ⚙️ Workflow Steps

### 1️⃣ Data Loading & Basic Preprocessing

-   Loaded dataset using Pandas
-   Dropped unnecessary columns (if present)
-   Separated features (X) and target (y)

### 2️⃣ Train-Test Split

-   80% Training Data
-   20% Testing Data
-   Stratified split to maintain class balance

### 3️⃣ Baseline Model

-   RandomForestClassifier with default parameters
-   Pipeline used with StandardScaler

### 4️⃣ Hyperparameter Tuning

-   Used GridSearchCV
-   5-Fold Cross Validation
-   Parameter Grid:
    -   n_estimators
    -   max_depth
    -   min_samples_split
    -   min_samples_leaf

### 5️⃣ Best Model Extraction

-   Extracted best parameters
-   Retrieved best trained estimator

### 6️⃣ Model Evaluation

Metrics Used: - Accuracy - Precision - Recall - F1-Score -
Classification Report

### 7️⃣ Model Comparison

-   Compared Default Random Forest vs Tuned Random Forest
-   Observed performance improvements

------------------------------------------------------------------------

## 📊 Expected Performance

Random Forest performs strongly on Breast Cancer dataset with accuracy
typically above 95%.

------------------------------------------------------------------------

## 💾 Saved Model

Best tuned model saved as:

tuned_rf_model.pkl

To load the model:

``` python
import joblib
model = joblib.load("tuned_rf_model.pkl")
```

------------------------------------------------------------------------

## 🛠 Tools & Libraries

-   Python
-   Pandas
-   Scikit-learn
-   Joblib
-   Google Colab

------------------------------------------------------------------------

## 📎 Project Type

Machine Learning -- Classification & Hyperparameter Tuning
