# Pima Indian Diabetes Analysis

This project uses the [Pima Indians Diabetes Database](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) from the National Institute of Diabetes and Digestive and Kidney Diseases. The goal is to predict whether a patient has diabetes or not based on various diagnostic measurements. All the patients are females above 21 years old and are of Pima Indian heritage.

---

## Data Information

| Feature                  | Description                                                        |
|--------------------------|--------------------------------------------------------------------|
| **Pregnancies**          | Number of times pregnant                                          |
| **Glucose**              | Glucose concentration 2 hours into an oral glucose tolerance test |
| **BloodPressure**        | Blood pressure (mm Hg)                                            |
| **SkinThickness**        | Skin fold thickness (mm)                                          |
| **Insulin**              | 2-Hour serum insulin (mu U/ml)                                    |
| **BMI**                  | Weight (kg) / [Height (m)]²                                       |
| **DiabetesPedigreeFunction** | Diabetes pedigree function (a function which scores likelihood of diabetes based on family history) |
| **Age**                  | Age (years)                                                        |
| **Outcome**              | Diabetes indicator (0 = No, 1 = Yes); 268 of 768 are “1”          |

---

## Confusion Matrix

|                     | Predicted = 1 | Predicted = 0 |
|---------------------|--------------:|--------------:|
| **Actual = 1**      | 66 (TP)       | 19 (FN)       |
| **Actual = 0**      | 24 (FP)       | 122 (TN)      |

- **True Positive (TP)**: Model correctly predicts diabetes.  
- **False Positive (FP)**: Model predicts diabetes, but the patient does not have it.  
- **True Negative (TN)**: Model correctly predicts no diabetes.  
- **False Negative (FN)**: Model predicts no diabetes, but the patient actually has it.

---

## Conclusion

- **Glucose**, **BMI**, and **Age** provide the most relevant information for distinguishing between patients with and without diabetes.
- Among the various machine learning models evaluated, the **Decision Tree** classifier delivered the best performance:
  - **Model Accuracy**: 
    - 76% on training data  
    - 81% on test data
  - **Precision (diabetes = 1)**: 78%  
    **Recall (diabetes = 1)**: 73%  
    **F1 Score (diabetes = 1)**: 75%
  - **Precision (diabetes = 0)**: 84%  
    **Recall (diabetes = 0)**: 87%  
    **F1 Score (diabetes = 0)**: 85%

---
