# Heart Disease Prediction
![](Screenshot_1.png)
 
## Introduction

1. This project is based on the dataset Heart Desease from UCI Machine Learning Repository and intends to predict if a person has or not heart desease. This would help in early detection of heart disease and hopefully serve as an aid in prevention of disease.

2. The dataset was collected from Kaggle (https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

## Dataset
This dataset contains information as related below and states the presence or not of heart disease.One of the most important column is 'target' which shows if an individuo has or not heart disease:
 - **age** : age of the patient [years]
 - **sex** : sex of the patient [1: Male, 0: Female]
 - **cp** : chest pain type [1: Typical Angina, 2: Atypical Angina, 3: Non-Anginal Pain, 4: Asymptomatic]
 - **trestbps** : resting blood pressure [mm Hg]
 - **chol** : serum cholesterol [mm/dl]
 - **fbs** : fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
 - **restecg** : resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
 - **thalach** : maximum heart rate achieved [Numeric value between 60 and 202]
 - **exang** : exercise-induced angina [Y: Yes, N: No]
 - **oldpeak** : oldpeak = ST [Numeric value measured in depression]
 - **slope** : the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
 - **ca** : the number of major vessels (0-3)
 - **thal** : a blood disorder called thalassemia [3: normal, 6: fixed defect, 7: reversable defect]
 - **target** : heart disease [0: no, 1: yes]
 
 ## Training and Prediction
We can train our model based on the existing data, as we have previously known if a patient has or not heart disease. This is referred to as supervision and learning.

### Preparing Machine Learning Models
#### By using:
- get_dummies in order to convert categorical variables into dummy (0 or 1)
- splitting train and test (20/80)
- accuracy_score

### Machine Learning Models used:
- LogisticRegression
- DecisionTreeClassifier
- AdaBoostClassifier
- KNeighborsClassifier
- RandomForestClassifier
And StandarScaler to try to improve each above model 

## Conclusion

According to the Classification Report, there is no big diference by using StandardScaler. Only KNeighbors has shown significant change from 60.34 to 77.59 (as models not based on `DecisionTreeClassifiers` are benefited)

`LogisticRegression` brought the best result to predict if a person has or not heart disease.
