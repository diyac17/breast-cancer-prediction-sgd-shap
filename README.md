# Breast Cancer Prediction using SGD with Explainable AI

## Overview
This project presents an explainable machine learning framework for breast cancer prediction using the **Breast Cancer Wisconsin (Diagnostic) dataset**.

The model is built using **Stochastic Gradient Descent (SGD)** and evaluated against **Logistic Regression** and **Random Forest** classifiers.

The framework integrates **Explainable AI (XAI)** techniques using **SHAP (SHapley Additive Explanations)** to interpret predictions and identify key tumor features influencing the model.

---

## Dataset
Breast Cancer Wisconsin (Diagnostic) Dataset  

- Samples: 569  
- Malignant: 212  
- Benign: 357  
- Features: 30 numerical attributes describing cell nuclei  

Source: UCI Machine Learning Repository / Kaggle

---

## Methodology
The workflow includes:

1. Data preprocessing and feature normalization  
2. Train-test split (80/20)  
3. Model training using:
   - SGD Classifier
   - Logistic Regression
   - Random Forest
4. Model evaluation using:
   - Accuracy
   - Precision
   - Recall
   - F1 Score
   - ROC-AUC
5. Model explainability using **SHAP analysis**

---

## Results

| Model | Accuracy | F1 Score | ROC-AUC |
|------|------|------|------|
| SGD-log | 0.974 | 0.964 | 0.985 |
| Random Forest | 0.974 | 0.963 | 0.993 |
| Logistic Regression | 0.965 | 0.951 | 0.996 |

The SGD model achieved strong predictive performance while maintaining computational efficiency and interpretability.

---

## Explainable AI (SHAP)

SHAP analysis revealed that the most influential tumor features include:

- concave points
- concavity
- texture
- radius
- area

These features align with established clinical indicators of malignancy.

---

## Files in Repository

data.csv → Breast Cancer dataset
ResearchPaper.pdf → Full research study
README.md → Project documentation

---

## Author

**Diya Chauhan**  
Machine Learning | Data Science | Healthcare AI

---

## Future Work

Future improvements may include:

- Integration of imaging datasets (mammograms, ultrasound)
- Multi-modal learning combining clinical and genomic data
- Deployment as a clinical decision-support tool
