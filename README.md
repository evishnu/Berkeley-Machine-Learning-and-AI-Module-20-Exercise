# Predicting Hospital Readmission in Diabetes Patients  
**Notebook**: `Model_Comparison_Readmission-confusionmatrice-roc-curves-aucscore.ipynb`

## 📘 Project Overview
This notebook is part of a healthcare-focused capstone project that aims to predict **30-day hospital readmissions** in diabetes patients using structured EHR data. The objective is to compare multiple classification algorithms and evaluate their effectiveness using confusion matrices, ROC curves, and AUC scores.


## Dataset
- **Source**: [UCI Machine Learning Repository - Diabetes 130-US hospitals dataset](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- **File used**: `diabetic_data.csv`
- **Size**: ~100,000 patient records
- **Target**: Readmission within 30 days (`readmitted_30`)



## Preprocessing Steps
- Removed features with excessive missing values: `weight`, `payer_code`, `medical_specialty`
- Transformed target variable to binary (`<30` → 1, otherwise 0)
- Dropped high-cardinality categorical variables
- Encoded `age` using label encoding
- Standardized numerical features using `StandardScaler`



## Models Compared
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **K-Nearest Neighbors (KNN)**
- **Note: I have compared the models using first 10,000 rows of the diabetic_Data.csv

Each model is evaluated using:
- Train & test accuracy  
- Training time  
- Confusion Matrix  
- ROC Curve and AUC Score



## Visualizations
- **Confusion Matrices**: To examine class-level prediction performance
- **ROC Curves**: To compare model sensitivity and specificity
- **AUC Scores**: For overall performance comparison
- **Note: Visualizations were created using first 10,000 rows of the diabetic_Data.csv



## 📂 File Structure
├── MLModels_Patient_Readmission.ipynb
├── diabetic_data.csv
├── confusion_matrix_Logistic_Regression.png 
├── confusion_matrix_Random_Forest.png 
└── roc_curves_all_models.png 
└── README.md

## Enhancement Considerations: This notebook uses default hyperparameters for all models.
#### Improve performance using cross-validation and hyperparameter tuning (e.g., GridSearchCV). Suitable for binary classification and healthcare ML demonstrations.
#### Include other Models based on future learning and feedbacks

## Contact: 
#### For questions or collaboration, reach out at: evishnu.shukla@gmail.com





