Pancreatic Cancer Prediction Models

This repository contains two different Jupyter notebooks for predicting pancreatic cancer diagnoses from urinary biomarker data:
	
	1.	Pancreatic_Cancer_DecisionTree_Classifier_Prediction_Model.ipynb
       •	Uses a single Decision Tree classifier (with hyperparameter tuning) to predict whether a patient has Pancreatic Ductal Adenocarcinoma, Benign Hepatobiliary Disease, or is a control (no pancreatic disease).
       •	Includes standard data preprocessing steps, model training, evaluation metrics, a confusion matrix, and a decision tree plot.
       
	2.	Pancreatic_Cancer_Stacked_Ensemble_RF_HGB_LR_Prediction_Model.ipynb
       •	Implements a stacked ensemble approach using:
       •	RandomForest and HistGradientBoosting as base estimators, and LogisticRegression as the final meta-learner.
       •	Includes standard performance evaluations (accuracy, classification report, confusion matrix) and a permutation-based feature importance analysis.
