# XGBoost Disease Diagnosis (Diabetes Prediction)

This project predicts whether a patient is likely to have diabetes using the *Pima Indians Diabetes dataset*.  
It compares a baseline model (*Random Forest) with **XGBoost (gradient boosting)* and evaluates performance using:
•⁠  ⁠Accuracy
•⁠  ⁠Classification Report (Precision, Recall, F1-score)
•⁠  ⁠ROC-AUC (optional)
•⁠  ⁠Confusion Matrix
•⁠  ⁠Feature Importance

## Dataset
•⁠  ⁠Source: Pima Indians Diabetes Dataset (loaded from a public URL in the notebook)
•⁠  ⁠Target column: ⁠ Outcome ⁠
  - ⁠ 0 ⁠ = No Diabetes
  - ⁠ 1 ⁠ = Diabetes

## Models Used
•⁠  ⁠*RandomForestClassifier* (baseline)
•⁠  ⁠*XGBoost (XGBClassifier)* (final model)

## Evaluation Metrics (What they mean)
•⁠  ⁠*Accuracy*: Overall % of correct predictions
•⁠  ⁠*Precision*: When the model predicts diabetes, how often it’s correct
•⁠  ⁠*Recall*: Out of all true diabetes cases, how many the model detects (important in healthcare)
•⁠  ⁠*F1-score*: Balance of precision and recall
•⁠  ⁠*Confusion Matrix*: Shows TP, TN, FP, FN
•⁠  ⁠*Feature Importance*: Highlights which features most influenced predictions

## How to Run

### Option 1: Run in Google Colab (Recommended)
Click below to open and run in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
[https://colab.research.google.com/drive/1uvH1S_U-isy0zt7-27aPrQ61ArQ3vH1I#scrollTo=UBIqP2HZY-2E](https://colab.research.google.com/drive/1pN1sXItq4POBiO7l3syfDvplnrRLdQoG)


## Results

•⁠  ⁠Random Forest Accuracy: 0.78  
•⁠  ⁠XGBoost Accuracy: 0.84  
•⁠  ⁠XGBoost Recall (Diabetes class): 0.82  
•⁠  ⁠F1 Score: 0.83  

XGBoost performed better than the baseline Random Forest model,
especially in recall for the positive (diabetes) class.

## Business / Healthcare Relevance

In healthcare, recall is especially important because failing to detect
a true diabetes case (false negative) can delay treatment and increase risk.
Therefore, improving recall for the positive class was prioritized over accuracy alone.
