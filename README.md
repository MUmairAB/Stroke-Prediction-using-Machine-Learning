# Stroke Prediction using Machine Learning

According to the [World Health Organization (WHO)](https://www.who.int/news-room/fact-sheets/detail/the-top-10-causes-of-death#:~:text=Stroke%20and%20chronic%20obstructive%20pulmonary,6%25%20of%20total%20deaths%20respectively.). stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths. This repository is a comprehensive project focusing on the prediction of strokes using machine learning techniques. The main objective of this project is to develop an accurate and reliable machine-learning model that can predict the likelihood of an individual experiencing a stroke.

The code provided in the repository offers a practical implementation of the machine learning models, enabling users to understand the workflow, data preprocessing steps, feature engineering techniques, model training, and evaluation. It serves as a valuable resource for researchers, data scientists, and enthusiasts interested in exploring stroke prediction using machine learning.

## 1. Dataset

The dataset used for the model training can be accessed on [Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset). This dataset labels whether a patient is likely to get a stroke based on the following input parameters:

1. id: unique identifier
2. gender: "Male", "Female" or "Other"
3. age: age of the patient
4. hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5. heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6. ever_married: "No" or "Yes"
7. work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8. Residence_type: "Rural" or "Urban"
9. avg_glucose_level: average glucose level in blood
10. bmi: body mass index
11. smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
12. stroke: 1 if the patient had a stroke or 0 if not

## 2. Images

The following images were created during the creation of this project.

#### 2.1 Heatmap of NULL values

<img src="https://github.com/MUmairAB/Stroke-Prediction-using-Machine-Learning/blob/main/Images/Heatmap%20of%20Null%20Values.png?raw=true" style="height: 453px; width:632px;"/>

#### 2.2 Target Analysis / Distribution of stroke data

<img src="https://github.com/MUmairAB/Stroke-Prediction-using-Machine-Learning/blob/main/Images/Distribution%20of%20stroke%20data.png?raw=true" style="height: 432px; width:580px;"/>


#### 2.3 Distribution of stroke values against BMI and Age

<img src="https://github.com/MUmairAB/Stroke-Prediction-using-Machine-Learning/blob/main/Images/Stroke%20Distribution%20Based%20on%20Bmi%20and%20Age.png?raw=true" style="height: 354px; width:953px;"/>

#### 2.4 Distribution of stroke values against BMI and Glucose Level

<img src="https://github.com/MUmairAB/Stroke-Prediction-using-Machine-Learning/blob/main/Images/Stroke%20Distribution%20Based%20on%20Bmi%20and%20Glucose%20Level.png?raw=true" style="height: 354px; width:953px;"/>


#### 2.5 Distribution of stroke values after balancing the dataset

As shown in Figure 2.2, the stroke data is highly imbalanced. So it was balanced through **SMOTE Upsampling**. The following piechart drawn using Plotly shows the balanced data.

<img src="https://github.com/MUmairAB/Stroke-Prediction-using-Machine-Learning/blob/main/Images/Dataset%20distribution%20after%20balancing.png?raw=true" style="height: 525px; width:676px;"/>

## How to use this model

The final trained model is saved using the **pickle** module. Moreover, a Python library was created using this model and was uploaded to Python's Open-Source repository of software, **PyPI** to better contribute to the community. The repository containing all the code about how to convert this model to a Python library is available in [this repo](https://github.com/MUmairAB/BrainStrokeClassifier).

You can install this model's Python library using:
```
 !pip install BrainStrokeClassifier
```


**By making the repository available on GitHub, the author promotes collaboration and encourages others to contribute to the project. Users can offer suggestions, provide enhancements, and even propose alternative models or approaches to improve the stroke prediction system to fuel advancements in stroke prediction research.**
