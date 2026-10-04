# Medical Risk Detection System

## Overview
This repository contains a machine learning pipeline designed to analyze patient data and predict high-risk medical cases. Because missing a high-risk patient is dangerous in a healthcare setting, the project heavily prioritizes **Recall** alongside overall accuracy during model evaluation.

---

## Models Evaluated
The project implements and tests multiple classification algorithms, ranging from baseline models to advanced ensemble techniques:
1. **Logistic Regression** (with $L2$ Regularization)[cite: 1]
2. **K-Nearest Neighbors (KNN)**[cite: 1]
3. **Random Forest Classifier** (Ensemble Learning)[cite: 1]
4. **Gradient Boosting Classifier** (Ensemble Learning)[cite: 1]
5. **Voting Classifier** (Soft voting combining Logistic Regression, KNN, and Random Forest)[cite: 1]

---

## Results & Performance Summary

| Model | Recall | Accuracy |
| :--- | :---: | :---: |
| **Logistic Regression** | 82.8%[cite: 1] | 81.4%[cite: 1] |
| **KNN** | 88.3%[cite: 1] | 88.3%[cite: 1] |
| **Voting Classifier** | 93.07%[cite: 1] | 91.5%[cite: 1] |
| **Gradient Boosting** | 94.9%[cite: 1] | 93.0%[cite: 1] |
| **Random Forest** | **95.8%**[cite: 1] | **93.8%**[cite: 1] |

### Key Takeaway
* **Best Performing Model:** **Random Forest** achieved the highest recall (**95.8%**) and accuracy (**93.7% / 93.8%**), making it the recommended choice for detecting high-risk patient targets[cite: 1].

---

## Requirements & Dependencies
To run this project, make sure you have the following Python libraries installed:

```bash
pip install pandas numpy scikit-learn
