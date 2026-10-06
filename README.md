# BCG-Data-Science-Job-Simulation-Customer-Churn-Analysis
BCG job simulation project focused on customer churn analysis, feature engineering, and Random Forest modeling with classification model evaluation.

## Overview

This project was completed as part of the **BCG Data Science Job Simulation** on Forage.

The project focuses on analyzing customer churn for an energy company using exploratory data analysis, feature engineering, and machine learning.

The workflow followed:

**Clean Dataset → EDA / Data Understanding → Feature Engineering → Modeling & Evaluation**

##  Project Objective

The objective was to understand customer churn patterns, prepare relevant features, and develop a machine learning model to identify customers at risk of churning.

## Project Workflow

### 1. Data Understanding & EDA

- Explored the provided clean dataset
- Analyzed customer and consumption-related variables
- Examined data structure and feature characteristics
- Identified potential patterns relevant to customer churn

### 2. Feature Engineering

Engineered additional features to improve the dataset for modeling, including:

- Activation date features
- Contract end date features
- Product modification date features
- Renewal date features
- Total consumption over 12 months
- Gas consumption share over 12 months

The final feature-engineered dataset contained **14,606 rows and 58 columns**.

### 3. Machine Learning Model

A **Random Forest Classifier** was developed to predict customer churn.

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

###  Model Limitation

Although the model achieved 90.31% accuracy, the recall was relatively low at 5.46%. This indicates that the model identified only a small proportion of the actual churn cases in the evaluation dataset. Therefore, accuracy alone should not be used to assess churn prediction performance, and further improvements such as class-imbalance handling, threshold optimization, or alternative modeling approaches could be explored.

##  Model Results

| Metric | Score |
|---|---:|
| Accuracy | 90.31% |
| Precision | 71.43% |
| Recall | 5.46% |
| F1-Score | 10.15% |
| ROC-AUC | 0.6649 |

### Confusion Matrix

```text
[[3278    8]
 [ 346   20]]
