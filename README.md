# Cardiovascular-Risk-Prediction

## Problem statement

The dataset is from an ongoing cardiovascular study on residents of the town of Framingham, Massachusetts. The classification goal is to predict whether the patient has a 10-year risk of future coronary heart disease (CHD). The dataset provides the patients’ information. It includes over 4,000 records and 15 attributes.

## Data Description

Demographic:
*  Sex: male or female("M" or "F")
*  Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to
whole numbers, the concept of age is continuous)

Behavioral:
*  is_smoking: whether or not the patient is a current smoker ("YES" or "NO")
* Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be
considered continuous as one can have any number of cigarettes, even half a cigarette.)

Medical( history):
* BP Meds: whether or not the patient was on blood pressure medication (Nominal)
* Prevalent Stroke: whether or not the patient had previously had a stroke (Nominal)
* Prevalent Hyp: whether or not the patient was hypertensive (Nominal)
* Diabetes: whether or not the patient had diabetes (Nominal)

Medical(current):
* Tot Chol: total cholesterol level (Continuous)
* Sys BP: systolic blood pressure (Continuous)
* Dia BP: diastolic blood pressure (Continuous)
* BMI: Body Mass Index (Continuous)
* Heart Rate: heart rate (Continuous - In medical research, variables such as heart rate though in
fact discrete, yet are considered continuous because of large number of possible values.)
* Glucose: glucose level (Continuous)

Target variable:
* 10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”) - Target variable

##Data Preprocessing & Feature engineering

1. Droping irrelevant features
2. Handling null values
3. Checking duplicate values
4. Dealing with outliers
5. Combining columns
6. Categorical encoding
7. Renaming Target Variable

## Exploratory Data Analysis

1. Univariate analysis
2. Bivariate analysis

## Conclusion - EDA

1. The dataset contains 85% normal persons and 15% heart patients
2. Given dataset consists of 55% male and 45% female.
3. Males are more prone to heart disease as compared to females.
4. As age increases, the chances of suffering from heart problems are more likely.
5. Higher BMI leads to higher chances of Heart Disease.
6. Higher cholesterol indicates the higher chances of getting Heart Disease.
7. If the value of MAP is above 96, the patient is more prone to Heart Disease or suffer Hypertension
8. People who take Blood pressure medication have a higher chance of suffering from heart disease.
9. People who previously had a stroke are more likely to suffer from Heart Disease.
10. Diabetic person is more likely to suffer from a heart disease.

## Steps to create Models

1. Dividing data into independent and dependent variables
2. Handle imbalancing of dataset using SMOTE
3. Train test split
4. Data Standerdization 
5. Creating models

## Different types of models created in colab
1. Logistic Regression
2. KNN
3. Decision Tree
4. Random Forest
5. Gradient Boost
6. XG Boost
7. Naive bayes classifier
8. Support Vector classifier

#Conclusion - Model
1. According to **Decision Tree and Random forest model**, **age** is the most important feature but according to **gradient boost and XG boost model**, most important features are **heart rate and sex respectively**.
2. **Gradient boost model is the most accurate model** among  all the models, on the basis of evaluation parameters such as  **Accuracy (90%), Precision (91%), Specificity (93%), F1 score (89%), and AUC-ROC score (96%)**.
3. **KNN model** is the best model on the basis of **Recall (93%)**.
4. **Logistic Regression model** has the least **Accuracy (70%)**.
