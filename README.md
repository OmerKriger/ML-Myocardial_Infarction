# Myocardial Infarction: A Machine Learning Approach
 
  ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas)![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)![matplotlib](https://img.shields.io/badge/matplotlib-2C5BB4?style=for-the-badge&logo=matplotlib&logoColor=white)![seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=Seaborn&logoColor=white)![shap](https://img.shields.io/badge/SHAP-FF0033?style=for-the-badge&logo=SHAP)![XGBoost](https://img.shields.io/badge/XGBoost-FF8300?style=for-the-badge&logo=xgboost)

**Authors**: Omer Kriger and Nir Peretz  
**Advisors**: Prof. Adi Shraibman, Dr. Dorit Shveiki, Dr. Yonatan Bilu  
**Institution**: The Academic College of Tel Aviv-Yaffo

## Overview

This project focuses on developing a predictive model using machine learning to assess the risk of Myocardial Infarction (MI), commonly known as a heart attack. MI occurs when blood flow to a part of the heart is blocked for a prolonged period, resulting in tissue damage. Early identification of high-risk individuals could lead to timely treatment and better patient outcomes.

## Dataset

- **Source**: UK Biobank  
- **Participants**: Over 500,000  
- **Features**: The dataset includes physical measurements, biological samples, medical history, lifestyle factors, and socio-demographic data.  
- **Target Variable**: MI diagnosis (binary outcome)

## Project Goals

1. **Predictive Modeling**: Develop a model that predicts the risk of MI using machine learning techniques.
2. **Feature Analysis**: Analyze the dataset to identify significant predictors of MI.
3. **Awareness and Preparedness**: Enhance early awareness and preparedness for potential treatment.

## Data Preprocessing

- **Exclusions**: Approximately 50% of participants diagnosed with MI were excluded, as their MI occurred before entering the UK Biobank. This ensures that the model’s features are not influenced by pre-existing conditions.
- **Data Split**: The dataset was split into training (70%), testing (20%), and validation (10%) sets.

## Model Selection and Training

The following machine learning models were used for training:

- **XGBoost**
- **Random Forest**

### Model Evaluation Techniques

- **Cross-validation**: K-fold cross-validation
- **Regularization**: L1 and L2 regularization
- **Evaluation Metrics**:
  - F1 Score
  - Recall and Precision
  - ROC Curve

## Results

The model faced challenges due to the limited representation of MI cases (2% of the dataset). Despite this, the model performed reasonably well in predicting both true negatives and true positives, indicating its effectiveness in identifying MI and non-MI cases for most of the dataset.

The confusion matrix for the test set showed:

- **True Negatives**: 62,585 (65.59%)
- **False Positives**: 32,834 (34.41%)
- **False Negatives**: 874 (30.44%)
- **True Positives**: 1,997 (69.56%)

Although the performance surpassed random guessing, further refinement of the model is necessary.

## Conclusion

This project demonstrates the challenges of using machine learning to predict MI due to the limited representation of positive cases. However, it also highlights the potential for machine learning to contribute to early detection and treatment strategies for myocardial infarction.

## Future Work

- **Model Optimization**: Further tuning of hyperparameters and exploration of more advanced algorithms.
- **Feature Engineering**: Identifying new features or transformations that could improve the model’s performance.
- **Handling Imbalance**: Explore techniques such as SMOTE or other methods for dealing with the imbalance in the dataset.
