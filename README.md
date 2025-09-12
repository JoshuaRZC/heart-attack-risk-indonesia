# Heart Attack Risk Prediction in Indonesia

This project analyzes **250,000 Indonesian health records** to quantify heart attack risk using advanced statistical methods and machine learning models. The focus is on identifying key clinical risk factors and developing a robust prediction model that outperforms traditional baselines.

---

## 📌 Project Overview
- **Objective**: Quantify heart attack risk and uncover major clinical risk factors.  
- **Dataset**: 250K anonymized Indonesian health records.  It can be downloaded from [Heart Attack Risk Prediction in Indonesia Dataset](https://www.kaggle.com/datasets/ankushpanday2/heart-attack-prediction-in-indonesia/data).
- **Key Results**:  
  - Identified **7 significant risk factors** (e.g., hypertension, diabetes, obesity, smoking). 
  - Achieved **72.3% prediction accuracy**, outperforming benchmarks such as Logistic Regression, SVM, Decision Trees, and Random Forests.  

---

## 🛠️ Methodology

1. **Feature Selection & Statistical Analysis** 
   - Visualized data and conducted data exploratory analysis using kernel density estimation.
   - Applied Spearman rank correlation tests and Kolmogorov–Smirnov test to identify candidate risk factors.
   - Controlled false discovery rate with Benjamini–Hochberg correction.  
   - Removed redundant predictors via VIF analysis. 
   
2. **Modeling** 
   - Implemented **Nadaraya–Watson kernel regression** with cross-validated bandwidth.  
   - Constructed **bootstrap-based confidence intervals** for robust uncertainty estimation.  

3. **Benchmarking** 
   - Compared against Logistic Regression, SVM, and XGBoost.  
   - Achieved **72.3% prediction accuracy**, outperforming all baseline models.  

---

## 🚀 Environment Setup
This project uses **Python 3.12**.  
To reproduce the environment:

```bash
conda env create -f environment.yml
conda activate heart_attack_pred
```