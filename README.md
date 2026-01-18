# feature-engineered-heart-disease-ml
Machine learning pipeline for heart disease prediction using Yeo-Johnson transformation, model comparison, and cross-dataset validation.


# ❤️ Early Heart Disease Prediction Using Machine Learning

This repository presents a complete and reproducible machine learning system for **early prediction of heart disease** using feature engineering and supervised learning models. The system is trained and evaluated on the Cleveland dataset and externally validated on the Statlog dataset to ensure generalization and reliability.

---

## 🎯 Project Goal

To build a **clean, stable, and accurate machine learning pipeline** capable of predicting heart disease risk using two independent datasets:

- Cleveland dataset → training & testing  
- Statlog dataset → external validation  

---

## 📊 Key Results (Summary)

- Data cleaning, Yeo-Johnson transformation, and feature scaling significantly improved data quality.
- **Random Forest** achieved the highest Accuracy, F1-score, and AUC on both datasets.
- **Logistic Regression** showed strong and consistent performance.
- **Decision Tree** performed weakest among the three models.
- Strong performance on the external dataset confirms good model generalization and low overfitting.

---

## 🧪 Scientific Interpretation

- Feature cleaning and transformation help models detect meaningful medical risk patterns.
- Random Forest performs best due to its ability to combine multiple trees and capture complex nonlinear relationships.
- External validation demonstrates that the system is robust and reliable.
- This project confirms that machine learning can effectively support **early and accurate heart disease prediction**.

---

## 🛠 Machine Learning Models Used

### 1. Logistic Regression
Predicts class probability using the sigmoid function:

P(Y = 1) = 1 / (1 + e^(−(β₀ + β₁X)))

---

### 2. Decision Tree
Splits data using Information Gain:

Information Gain = Entropy(before split) − Entropy(after split)

---

### 3. Random Forest
Combines predictions from many decision trees:

Final Prediction = Majority Vote of All Trees

---

## 📈 Model Evaluation

### ROC Curve
Plots True Positive Rate vs False Positive Rate:

TPR = TP / (TP + FN)  
FPR = FP / (FP + TN)

### AUC Score
Measures overall classification performance:

AUC = Area Under the ROC Curve

---

## 🔄 Feature Transformation

### Yeo-Johnson Transformation

Used to reduce skewness and normalize features:

For X ≥ 0:  
Y = ((X + 1)^λ − 1) / λ  

For X < 0:  
Y = −((1 − X)^(2 − λ) − 1) / (2 − λ)

---

## 🧭 Project Workflow

1. Load Cleveland and Statlog datasets  
2. Data cleaning and preprocessing  
3. Train–test split  
4. Feature transformation (Yeo-Johnson) and scaling  
5. Model training (LR, DT, RF)  
6. Evaluation on Cleveland test set  
7. External validation on Statlog dataset  
8. Metric computation (Accuracy, Precision, Recall, F1, AUC)  
9. ROC curve and performance visualization  
10. Model comparison and final analysis  

---

## 🧰 Technologies Used

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## ⚠ Disclaimer

This project is for academic and research purposes only and does not replace professional medical diagnosis.

---

## 📌 Conclusion

This work demonstrates that properly engineered features combined with robust machine learning models—especially Random Forest—can provide reliable early heart disease risk prediction and support clinical decision-making.

---

