# Pima-Indian-Diabetes-Analysis

Pima Indian Diabetes Analysis This dataset is taken from National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the analysis is to predict whether the patient has diabetes or not based on the measurements given in the dataset. All the patients are females above 21 years old and belong to Pima Indian heritage.

### Data Information

Pregnancies: No of times pregnant

Glucose: Glucose concentration a 2 hours in an oral glucose tolerance test

BloodPressure: blood pressure (mm Hg)

SkinThickness: skin fold thickness (mm)

Insulin: 2-Hour serum insulin (mu U/ml)

BMI: weight in kg/(height in m)^2

DiabetesPedigreeFunction: pedigree function

Age: Age (years)

Outcome: variable (0 or 1) 268 of 768 are 1, the others are 0

### Conclusion

The features of Glucose, BMI, and age provide the most relevant information to distinguish between the true and false classes.

The Decision Tree classifier showed the best performance among all the models, achieving a model score of 76% on the training data and 81% on the test data. The model can predict with 78% precision whether a patient has diabetes, with a 73% recall and 75% F1 score. Similarly, it can predict with 84% precision whether a patient does not have diabetes, with an 87% recall and 85% F1 score.

The confusion matrix below provides an overview of the predictions:

True Positive (observed=1, predicted=1): 66
False Positive (observed=0, predicted=1): 24
True Negative (observed=0, predicted=0): 122
False Negative (observed=1, predicted=0): 19
A true positive means that the model correctly predicted that the patient has diabetes. A false positive means that the model predicted that the patient has diabetes, but in reality, the patient does not have it. A true negative means that the model correctly predicted that the patient does not have diabetes. A false negative means that the model predicted that the patient does not have diabetes, but in reality, the patient does have it.
