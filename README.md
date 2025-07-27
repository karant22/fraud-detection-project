# Fraud Detection Using Machine Learning

This project focuses on detecting fraudulent financial transactions using a real-world transactional dataset with over 6 million records. It demonstrates the end-to-end application of data science: from data cleaning and feature engineering to model building, evaluation, and insight generation.

# 📌 Project Highlights

- ✅ Cleaned and analyzed a large financial dataset (6M+ records)
- ✅ Handled missing values, outliers, and multicollinearity
- ✅ Performed feature engineering (encoding, scaling)
- ✅ Built a Random Forest classification model to detect fraud
- ✅ Evaluated performance using AUC, precision, recall, F1-score
- ✅ Identified top features and proposed fraud prevention strategies



# Files Included

 `Fraud_Detection.ipynb`-->Main Jupyter Notebook 
 `Fraud_Detection.pdf`-->Exported version of the notebook 
 `sample_data.csv`-->Sample dataset 
 `README.md`-->Project documentation 


#Tools & Technologies

- Python (Colab)
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- SHAP (for explainability)



# Model Evaluation

- AUC Score: ~0.93
- Precision: High (few false positives)
- Recall: High (detects most fraud cases)
- F1-Score: Balanced for fraud classification



# Key Findings

- Fraud is highly linked to:
  - High-value transactions
  - `TRANSFER` and `CASH_OUT` types
  - Source or destination accounts with zero balances

- These patterns align with typical fraud behavior like money laundering, account takeovers, and rapid fund movement

---

## 🔐 Suggested Prevention Measures

- Real-time fraud scoring with threshold-based blocking
- Delay or review for suspicious transaction types (e.g., `TRANSFER`)
- Monitor accounts with sudden balance changes or multiple transfers
- Add verification steps (e.g., OTP) for high-risk transactions

---

# 🔗 Dataset

Due to size limitations, the full dataset is not hosted in this repository.  
Download link:[Download Dataset](https://drive.google.com/file/d/13tUYS_NDUetZPMyjM7-Nr5VtJnWHMxKH/view?usp=sharing)


##🚀 Future Improvements

- Use advanced models like XGBoost or LightGBM
- Add real-time detection with a Streamlit dashboard
- Include temporal/behavioral features (e.g., transaction velocity)

