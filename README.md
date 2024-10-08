1- Dataset description

Data has been collected on a group of patients, who suffered from the same disease. During their course of treatment, each patient responded to one of 5 drugs, Drug A, Drug B, Drug C, Drug X, and Drug Y.

It is then possible to build a model to find out which drug might be appropriate for a future patient with the same disease. The characteristics of this data set are age, sex, blood pressure, cholesterol of the patients, Sodium to potassium ratio in blood of the patient and the target is the drug to which each of these patients responded.

It is a sample of a multiclass classifier, and you can use the training part of the dataset to build a decision tree and then use it to predict the class of an unknown patient or to prescribe a drug to a new patient.


There are 6 variables in this data set:

4 categorical variables and 2 continuous variables.

The feature sets are:

Age -> Patient Age
Sex -> Gender of patient (male or female)
BP -> Blood Pressure Levels of patient (high, normal, or low)
Cholesterol -> Cholesterol Levels of patient (high or normal)
Na_to_K -> Sodium to potassium ratio in blood of patient
Drug -> Type of drug
*****************************************************************************************************************************************
2- Objetives

For the development of the notebook, we will use a predictive technique through supervised learning for data analysis. This classification algorithm will be carried out through the decision tree technique.

Develop a classification model using Decision Tree Algorithm.
Develop an ensemble method using the Random Forest model.
Dataset exploration using various types of data visualization.
Implement the CRISP-DM methodology used in analytical projects.
*****************************************************************************************************************************************
3- Exploratory Data Analysis

3-1. Import the data.
3-2. Data exploration.
3-3. Statistics visualization and relations between the data.
3-4. Prepare the data.
*****************************************************************************************************************************************
4- Model Implementation

4-1 Decision Tree (Classifier Model).
4-2 Random Forest (Ensemble Method).
*****************************************************************************************************************************************
5- Conclusions

Descriptive Analysis:

- There is no direct relation between age and Na_to_K, in either of the two genders.
- DrugB is taken only by older than 51 years old.
- DrugA is taken only by younger than 50 years old.
- Male people get drugA and drugC more than femenil people.
- Female people get drugB and drugX more than male people.
- DrugY seems equal for male and female people.
- DrugA and DrugB are only given to people who have HIGH blood pressure.
- DrugC is only given to people who have LOW blood pressure.
- DrugX is given to people who have LOW and NORMAL(higher proportion) blood pressure.
- All patients no matter their BP can take the drugY.
- People who have Na_to_K ratio bigger or equal than 15.015, get DrugY.
- Peple who have Na_to_K ratio smaller or equal than 14.642, can get DrugC, DrugX, DrugA or DrugB.
- The people with HIGH cholesterol, only can take the drugC.
- It looks likes no matter if they have the cholesterol HIGH or NORMAL, they can take the drugA, drugB, drugX and drugY.
- If people have HIGH blood pressure and Na_to_K ratio is lower than 15, they get drugA and drugB only.
- If people have LOW blood pressure and Na_to_K ratio is lower than 15, they get drugC only.
- The drugX is not taken by people how have HIGH blood pressure.
- If people have HIGH cholesterol and Na_to_K ratio is lower than 15, they get drugC only.
- The drugC is not taken by people who have NORMAL cholesterol.

Predictive Analysis:

- The 3 most important attributes were Cholesterol, Sex and Sodium Potassium ratio in blood.
- The 2 less important attributes were Blood Pressure and Age.
- Based on the results, it can be said that both ML models have an accuracy of more than 95% in predicting classification of drug type.
- The choice model were decision tree, because it has more accuracy.
*****************************************************************************************************************************************
