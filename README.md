Pancreatic Cancer Prediction Models
-------------------------------

This repository provides two distinct Jupyter notebooks demonstrating how to predict pancreatic cancer diagnoses using urinary biomarker data. Each notebook employs a different approach in regards to its model, showcasing different approaches to the same problem. 
<br>
The goal is to classify patients into three categories of diagnosis classes they are defined as:

	1: Control (No Pancreatic Disease)
 	
	2: Benign Hepatobiliary Disease (including chronic pancreatitis)
 	
	3: Pancreatic Ductal Adenocarcinoma (Pancreatic Cancer)

Note: "Its highly recommend to click into the files and read through the results do not just rely on this README"!
	
	1.	Pancreatic_Cancer_DecisionTree_Classifier_Prediction_Model.ipynb
 
       •	Uses a single Decision Tree classifier (with hyperparameter tuning) to predict whether a patient has Pancreatic Ductal Adenocarcinoma, Benign Hepatobiliary Disease, or is a control (no pancreatic disease).
       •	Includes standard data preprocessing steps, model training, evaluation metrics, a confusion matrix, and a decision tree plot.
       
	2.	Pancreatic_Cancer_Stacked_Ensemble_RF_HGB_LR_Prediction_Model.ipynb
 
       •	Implements a stacked ensemble approach using:
       •	RandomForest and HistGradientBoosting as base estimators, and LogisticRegression as the final meta-learner.
       •	Includes standard performance evaluations (accuracy, classification report, confusion matrix) and a permutation-based feature importance analysis.

<br>

Dataset
-------------------------------
	•	The dataset is provided by [John J. Davis IV on Kaggle.](https://www.kaggle.com/datasets/johnjdavisiv/urinary-biomarkers-for-pancreatic-cancer)

<br>

In regards to the Pancreatic_Cancer_DecisionTree_Classifier_Prediction_Model.ipynb these are the results and outcomes of the model:
-------------------------------
Note: "It is possible to get higher results of accuracy etc when running it again yourself"!
<br>

Best hyperparameters: {'classifier__max_depth': 5, 'classifier__min_samples_leaf': 1, 'classifier__min_samples_split': 50}
<br>
Best CV accuracy: 0.633
<br>
Test accuracy (tuned): 0.644

Classification Report (tuned):

 		   precision    recall  f1-score   support
	1       	0.65      0.55      0.60        31
	2       	0.58      0.75      0.65        44
	3               0.74      0.60      0.67        43

	accuracy                            0.64       118
	macro avg       0.66      0.63      0.64       118
	weighted avg    0.66      0.64      0.64       118

<br>
The amount of randomly selected patients are: 35
<br>
Overall Accuracy on Random Samples: 0.771


<br>
<br>
<br>


In regards to the Pancreatic_Cancer_Stacked_Ensemble_RF_HGB_LR_Prediction_Model.ipynb these are the results and outcomes of the model:
-------------------------------
Note "It is possible to get higher results of accuracy etc when running it again yourself"!
<br>

Best hyperparameters: {'classifier__final_estimator__C': 10, 'classifier__hgb__max_iter': 200, 'classifier__rf__n_estimators': 100}
<br>
Best CV accuracy: 0.676
<br>
Test accuracy (tuned): 0.746

Classification Report (tuned):	

  		 precision    recall  f1-score   support
	1             0.71      0.77      0.74        31
	2             0.67      0.66      0.67        44
	3             0.85      0.81      0.83        43

	accuracy                          0.75       118
	macro avg     0.74      0.75      0.75       118
	weighted avg  0.75      0.75      0.75       118

<br>
The amount of randomly selected patients are: 25
<br>
Overall Accuracy on Random Samples: 0.960


Viewing Outputs and Results.
-------------------------------

To see the output/results of the run programs just click into the corrsponding file either:
<br>
Pancreatic_Cancer_Stacked_Ensemble_RF_HGB_LR_Prediction_Model.ipynb or Pancreatic_Cancer_DecisionTree_Classifier_Prediction_Model.ipynb 
<br>
and scroll all the way down to see the ouputs/results and all of the visualzations.


License
-------------------------------
This project is distributed under the MIT License. Refer to the LICENSE file for details.









