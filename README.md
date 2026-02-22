# Water-Potability-Datathon
Binary classification of water potability using ensemble ML models. Covers data preprocessing, imbalance handling with SMOTE, feature scaling, and hyperparameter tuning with balanced accuracy scoring.

# Water Potability Classification – Machine Learning Project

## Overview
This project focuses on predicting water potability using physicochemical properties through supervised machine learning techniques. The objective is to classify water samples as potable (safe for human consumption) or not potable based on various water quality indicators.

## Problem Statement
Access to safe drinking water is a critical public health concern. Using numerical measurements such as pH, hardness, solids, chloramines, sulfate, conductivity, organic carbon, trihalomethanes, and turbidity, the task is formulated as a binary classification problem:

- 1 → Potable  
- 0 → Not Potable  

## Data Preprocessing
The dataset contained missing values in multiple features. The following preprocessing steps were applied:

- Imputation using mean and median strategies depending on feature distribution.
- Train–test split to prevent data leakage.
- Feature scaling using StandardScaler.
- Class imbalance handling using SMOTE to improve minority class prediction.

## Modeling Approach
Multiple models were implemented and compared:

- Random Forest Classifier
- Gradient Boosting Classifier

Hyperparameter tuning was performed using GridSearchCV with balanced accuracy scoring to account for class imbalance.

## Evaluation Metrics
Model performance was evaluated using:

- Balanced Accuracy
- Accuracy
- Recall
- Specificity
- Confusion Matrix

The final model demonstrated improved minority class detection after applying SMOTE, highlighting the importance of addressing imbalance in health-related datasets.

## Key Learnings
- Proper imbalance handling significantly improves recall for minority classes.
- Tree-based ensemble methods perform well for structured tabular classification tasks.
- Balanced accuracy is a more reliable metric than standard accuracy in imbalanced datasets.

## Disclaimer
This repository represents the implementation and analysis of a datathon solution for learning and technical portfolio purposes.
