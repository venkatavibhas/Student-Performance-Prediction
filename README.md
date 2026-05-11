# Student Performance Prediction Using Machine Learning

## Project Overview

This project predicts students' final mathematics grade (G3) using the Student Performance Dataset.  
The goal is to understand which student background, academic, and behavior-related factors are associated with final performance.

This project was completed in two phases.  
Phase 1 included data loading, data audit, exploratory data analysis, preprocessing, baseline modeling, and error analysis.  
Phase 2 improved the project with stronger validation, feature engineering, model comparison, interpretability, fairness analysis, and a final decision-support deliverable.

## Dataset

Dataset: Student Performance Dataset - Mathematics  
Source: UCI Machine Learning Repository  
File used: `student-mat.csv`  
Target variable: `G3`, final mathematics grade

## How to Run

1. Open the final notebook in Google Colab.
2. Run all cells from top to bottom.
3. Upload `student-mat.csv` when prompted.
4. Review the EDA, baseline model, Phase 2 model comparison, interpretation, fairness analysis, and final decision memo.

## Methods Used

- Data audit
- Exploratory data analysis
- Preprocessing pipeline
- Ridge Regression baseline
- 5-fold cross-validation
- Feature engineering
- Model comparison
- Random Forest
- Gradient Boosting
- Permutation importance
- Fairness / slice analysis
- Responsible AI discussion

## Main Results

The best model with G1 and G2 included was Random Forest, with MAE around 1.03.  
The best model without G1 and G2 was also Random Forest, with MAE around 2.89.

This shows that previous grades are very strong predictors of final grade.  
However, G1 and G2 may create leakage or near-leakage because they are previous grades from the same course.

## Responsible AI

This model should be used only as decision support.  
It should not be used to punish, label, rank, or automatically make decisions about students.  
Educators should combine model results with teacher judgment and student context.

## Author

Aditham Venkata Vibhas  
DSA 502 Final Project
