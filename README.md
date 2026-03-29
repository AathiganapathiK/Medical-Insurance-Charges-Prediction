#  Medical Cost Prediction using Machine Learning

## Project Overview
This project focuses on predicting **medical insurance charges** using machine learning techniques. By analyzing patient details such as age, BMI, smoking status, and number of children, the model estimates healthcare costs.

The objective is to understand key factors influencing medical expenses and build a predictive model that can assist in cost estimation.

This project follows a complete **end-to-end data science workflow**, including data preprocessing, analysis, modeling, and evaluation.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Introduction](#introduction)
3. [Background and Motivation](#background-and-motivation)
4. [Dataset](#dataset)
5. [Workflow](#workflow)
6. [Machine Learning Models](#machine-learning-models)
7. [Model Evaluation](#model-evaluation)
8. [Performance Summary](#-performance-summary)
9. [Key Insights](#key-insights)
10. [Sample Predictions](#sample-predictions)
11. [Technologies Used](#technologies-used)
12. [Project Structure](#project-structure)
13. [How to Run the Project](#how-to-run-the-project)
14. [Conclusion](#conclusion)
---

## Introduction

Healthcare costs have been rising significantly, making it important to estimate medical expenses accurately. This project focuses on predicting **medical insurance charges** using machine learning techniques based on individual attributes such as age, BMI, smoking status, and number of dependents.

By analyzing these factors, the model aims to provide reliable cost predictions that can help individuals, insurance companies, and healthcare providers make informed financial decisions. This project demonstrates how data-driven approaches can improve cost estimation in the healthcare domain.

---

## Background and Motivation

Medical insurance charges vary widely depending on multiple personal and lifestyle factors. Traditional methods of estimating these costs often fail to capture complex relationships between variables such as smoking habits, age, and body mass index.

With the help of **machine learning**, it becomes possible to uncover hidden patterns in the data and build predictive models that provide more accurate estimations.

This project is motivated by the need to:
- Understand key factors influencing medical insurance costs  
- Analyze relationships between health attributes and expenses  
- Build predictive models for accurate charge estimation  
- Support better financial planning in healthcare  

By applying models like Linear Regression and Random Forest, this project highlights how machine learning can be effectively used to predict insurance costs and assist in decision-making.

---

## Dataset
The dataset used is the [**Medical Cost Personal Dataset**](https://www.kaggle.com/datasets/d3lhomi10/medical-cost-personal-dataset).

### Features:
- **age** – Age of the individual  
- **sex** – Gender (male/female)  
- **bmi** – Body Mass Index  
- **children** – Number of dependents  
- **smoker** – Smoking status (yes/no)  
- **region** – Residential region  
- **charges** – Medical insurance cost (target variable)  

The goal is to **predict the charges** based on these features.

---

## Workflow

### 1. Data Loading
- Loaded dataset using pandas  
- Displayed initial rows to understand structure  

---

### 2. Data Cleaning
- Introduced missing values for demonstration  
- Handled missing values using **median imputation**  
- Ensured dataset consistency  

---

### 3. Exploratory Data Analysis (EDA)
Performed analysis to understand data patterns and relationships.

#### Visualizations:
- Distribution of medical charges  
- BMI distribution  
- Smoker vs charges  
- Age vs charges  
- Correlation heatmap  

#### Observations:
- Charges are **right-skewed**  
- Smokers have significantly higher charges  
- Charges increase with age  
- BMI moderately affects cost  

---

## Machine Learning Models

### Linear Regression
- Simple baseline model  
- Assumes linear relationships  

### Random Forest Regressor
- Ensemble model  
- Handles complex and non-linear relationships  
- Provides better prediction accuracy  

---

## Model Evaluation

The following metrics were used:

- **R² Score** – Measures model performance  
- **MAE (Mean Absolute Error)** – Average prediction error  
- **RMSE (Root Mean Squared Error)** – Penalizes larger errors  

---

## Performance Summary

| Model | R² Score | MAE | RMSE |
|------|---------|------|------|
| Linear Regression | 0.8072 | $4176.560 | $5951.121 |
| Random Forest | 0.8786 | $2697.545 | $4721.292 |

> Random Forest performed better than Linear Regression.

---

## Key Insights

- Smoking is the **most important factor** affecting medical charges  
- Age has a strong positive relationship with cost  
- Higher BMI leads to increased medical expenses  
- Smokers incur significantly higher healthcare costs  

---

## Sample Predictions

The trained model was used to predict charges for new patient profiles.

- Non-smokers → lower predicted charges  
- Smokers → significantly higher predicted charges  

This demonstrates real-world applicability of the model.

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Jupyter Notebook  

---

## Project Structure

```
medical-insurance-charges-prediction/
│
├── Data/
│ ├── insurance.csv
│ ├── insurance_with_missing.csv
│ └── cleaned_dataset.csv
│
├── Notebook/
│ └── medical_cost_prediction.ipynb
│
└── README.md
```

---

## How to Run the Project

1. Clone the repository

```bash
git clone https://github.com/AathiganapathiK/Medical-Insurance-Charges-Prediction.git
```
2. Install required libraries
```
pip install pandas numpy matplotlib seaborn scikit-learn
```
3. Change Dataset path and Run the notebook
```
jupyter notebook
```
Open:
```
medical_cost_prediction.ipynb
```

---

## Conclusion

This project successfully predicts medical insurance charges using machine learning techniques.

Random Forest proved to be the most effective model due to its ability to capture complex relationships between features.

The project highlights how data-driven approaches can support better decision-making in healthcare and insurance industries.

---
