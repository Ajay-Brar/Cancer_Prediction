# Cancer_Prediction Model
# Breast Cancer Prediction using Machine Learning

This project implements a diagnostic tool to classify breast cancer tumors as either **Malignant** or **Benign** based on medical dataset features. It explores various supervised learning algorithms and optimizes them to achieve high diagnostic accuracy.

## 📌 Project Overview
The primary goal of this project is to leverage machine learning to assist in medical diagnosis. Early and accurate detection of breast cancer is critical for effective treatment planning. This repository covers:
- **Exploratory Data Analysis (EDA):** Visualizing feature correlations and class distributions.
- **Data Preprocessing:** Handling categorical labels using `LabelEncoder` and feature scaling with `StandardScaler`.
- **Model Comparison:** Evaluating multiple classifiers including Random Forest, SVM (Support Vector Machines), and others.
- **Hyperparameter Tuning:** Using `GridSearchCV` to find the optimal parameters (e.g., number of estimators) for peak performance.

## 📊 Dataset
The project utilizes a dataset containing clinical features of breast mass nuclei, such as:
- Radius, Texture, Perimeter, and Area.
- Smoothness, Compactness, Concavity, and Symmetry.
- **Target Variable:** Diagnosis (Malignant/Benign).

## 🛠️ Tech Stack
- **Language:** Python
- **Key Libraries:**
  - `Scikit-Learn`: For model building, cross-validation, and metrics.
  - `Pandas` & `NumPy`: For efficient data handling.
  - `Seaborn` & `Matplotlib`: For statistical data visualization and confusion matrices.

## ⚙️ Methodology
1. **Feature Engineering:** Standardization of numerical features to ensure all inputs contribute equally to the distance-based calculations.
2. **Model Training:** - Training a **Random Forest Classifier** and an **SVM** model.
   - Using **K-Fold Cross-Validation** to ensure the model's stability across different data splits.
3. **Optimization:** Implementing `GridSearchCV` to fine-tune the `n_estimators` for the Random Forest model.

## 📈 Evaluation Results
The models are evaluated based on:
- **Accuracy Score:** The percentage of correct classifications.
- **Confusion Matrix:** To analyze True Positives, True Negatives, and particularly False Negatives (critical in medical contexts).
- **Classification Report:** Detailed Precision, Recall, and F1-Score analysis.

The optimized Random Forest model in this notebook achieved an accuracy of approximately **99%**.

