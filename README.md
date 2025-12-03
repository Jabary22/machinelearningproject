# machinelearningproject
#  Healthcare Provider Fraud Detection Project  

This repository contains an end-to-end machine learning pipeline for detecting potentially fraudulent healthcare providers using the *Healthcare Provider Fraud Detection Dataset*.  
The project covers data preparation, feature engineering, class imbalance handling, model training, comparison, and evaluation.



## 1. Project Overview  

Healthcare fraud causes billions in losses every year.  
Our goal is to build a complete *fraud detection ML pipeline* capable of identifying healthcare providers whose claim patterns are suspicious or abnormal.

### Data Loading & Cleaning  
- Combined multiple CMS-like datasets (Beneficiary, Inpatient, Outpatient, Fraud Labels)  
- Handled missing values, duplicates, invalid types  
- Filtered irrelevant data  
- Built provider-level aggregated datasets

###  Feature Engineering  
- Created statistical summaries per provider (counts, averages, totals)  
- Added features related to diagnoses, procedures, chronic conditions  
- Encoded categorical fields and standardized numerical ones

###  Handling Class Imbalance  
Because fraudulent providers represent a very small percentage of the dataset, we experimented with:  
- SMOTE oversampling  
- Random undersampling  
- Class weights  

*Final chosen strategy:* (fill this based on your notebook results)

###  Model Training  
We trained and tested multiple algorithms:  
- Logistic Regression  
- Decision Tree  
- Random Forest  
- Gradient Boosting  
- XGBoost / LightGBM  

###  Model Evaluation  
We focused on metrics that matter for fraud detection:  
- Precision  
- Recall  
- F1-score  
- ROC-AUC  
- PR-AUC  
- Confusion Matrix  

---

##  2. Team Members  
 
 *Malak El Akkad* | *13004588* 
*Engy Mohamed* | *13003004* 
*Mahmoud Tahon* | *13001310* 
*Abdelrahman Tamer* | *10003179* 

---

##  3. Summary of Results  

###  Best Performing Model  
*(Fill this in — e.g., Random Forest or XGBoost)*

###  Test Set Metrics  
- *Accuracy:* X.XX  
- *Precision:* X.XX  
- *Recall (Fraud):* X.XX  
- *F1-Score:* X.XX  
- *ROC-AUC:* X.XX  

###  Interpretation  
- High recall ensures more fraudulent providers are detected.  
- Good precision reduces false accusations.  
- The model effectively identifies unusual claim behavior using engineered features.

---

##  4. Reproduction Instructions  

### *1️Clone the Repository*
```bash
git clone https://github.com/yourusername/fraud_detection_yourteam.git
cd fraud_detection_yourteam
