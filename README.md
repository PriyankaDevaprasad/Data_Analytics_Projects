# 🌲 Forest Cover Type Classification

## 📌 Project Overview

A Machine Learning classification project that predicts the **forest cover type** of a geographical location using cartographic and environmental features such as elevation, slope, soil type, wilderness area, and distances to hydrology, roads, and fire points.

## 🔄 Project Workflow

### 1. Data Collection

* Load the Forest Cover Type dataset using Pandas.
* Understand the dataset structure and features.

### 2. Data Understanding

* Check shape, data types, and statistical summary.
* Check missing values and duplicate records.
* Analyze target class distribution.

### 3. Data Cleaning & Transformation

* Handle missing values.
* Detect and handle outliers.
* Analyze and handle skewness.
* Prepare the data for Machine Learning.

### 4. Feature Engineering

* Encode categorical variables.
* Create useful derived features where required.
* Prepare features and target variable.

### 5. Exploratory Data Analysis (EDA)

* Analyze feature distributions.
* Study relationships between features.
* Analyze class distribution.
* Identify important features using visualizations and correlation analysis.

### 6. Class Imbalance Handling

* Analyze class imbalance in the target variable.
* Apply **SMOTE** to balance the training data.

### 7. Feature Selection

* Analyze feature importance.
* Identify relevant features.
* Remove less useful features where appropriate.

### 8. Model Building

Train and compare multiple classification algorithms:

* Random Forest
* Decision Tree
* Logistic Regression
* K-Nearest Neighbors (KNN)
* XGBoost

### 9. Model Evaluation

Evaluate the models using:

* Accuracy
* Macro F1-Score
* Weighted F1-Score
* Confusion Matrix
* Classification Report

### 10. Cross-Validation

* Apply **Stratified K-Fold Cross-Validation**.
* Compare model performance across multiple folds.

### 11. Hyperparameter Tuning

* Apply **GridSearchCV / RandomizedSearchCV**.
* Optimize the selected model's hyperparameters.

### 12. Final Model

* Select the final model based on evaluation results.
* Train the final model.
* Save the model using Pickle/Joblib.

### 13. Streamlit Deployment

* Build an interactive Streamlit application.
* Accept user inputs for forest-related features.
* Apply the saved preprocessing objects.
* Predict the forest cover type.

## 🛠️ Technologies Used

**Python | Pandas | NumPy | Matplotlib | Seaborn | Scikit-learn | SMOTE | XGBoost | Streamlit | Git & GitHub**

## 👩‍💻 Author
**Priyanka Chandrapaul**

