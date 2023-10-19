# Predicting Employee Attrition
#### *Analyzing Employee Retention and Constructing a Machine Learning Model*

*A case study by Waqas Ahmad*
## Overview

Mercedes-Benz's HR department is on a mission to boost employee satisfaction by uncovering the core factors that could trigger an employee's decision to leave the company.

## Goal

The goal of this project is to analyze the data collected by the HR department and develop a robust predictive model that can accurately forecast an employee's likelihood of leaving the company.

## Objective

The objective of this project is to identify factors that play a role in employees choosing to leave the company and suggest a way forward.


## Table of Contents
1. [Introduction](#introduction)
2. [Data Preprocessing](#data-preprocessing)
3. [Exploratory Data Analysis](#exploratory-data-analysis)
4. [Model Building and Evaluation](#model-building-and-evaluation)
5. [Feature Engineering](#feature-engineering)
6. [Conclusion and Recommendations](#conclusion-and-recommendations)
7. [Next Steps](#next-steps)



## 1. Introduction <a name="introduction"></a>

Employee attrition, or the phenomenon of employees leaving a company, is a critical issue that affects organizations in many ways. In this project, we aim to build predictive models to identify factors contributing to employee attrition and provide actionable insights to address this challenge. The project can be divided into four main stages:

- **Data Preprocessing**: In this stage, we prepared the data for analysis and modeling by addressing missing values, performing one-hot encoding, and isolating the outcome variable and features.

- **Exploratory Data Analysis (EDA)**: EDA is crucial for understanding the dataset, identifying patterns, and exploring potential features that may impact employee attrition. Various statistical and visual techniques were used to gain insights.

- **Model Building and Evaluation**: We constructed two types of machine learning models—Logistic Regression and Tree-Based Models (Decision Tree and Random Forest). These models were evaluated on various metrics to determine their effectiveness in predicting employee attrition.

- **Feature Engineering**: We addressed concerns about data leakage and improved model robustness by excluding the 'satisfaction_level' feature, creating a new binary feature called 'overworked,' and dropping the 'average_monthly_hours' feature.
## Project Stages

### Stage 1: Import Data & Packages
- Import necessary data and Python packages for analysis.

### Stage 2: Data Exploration - EDA & Data Cleaning
- Perform exploratory data analysis (EDA) and data cleaning to understand the dataset and prepare it for modeling.

### Stage 3: Building Models
- Explore two different approaches for building predictive models:
  - Approach A: Regression Modeling
  - Approach B: Tree-Based Modeling (Decision Tree & Random Forest)

### Stage 4: Model Evaluation & Sharing Insights
- Evaluate the models and share insights gained from them.

## 2. Data Preprocessing <a name="data-preprocessing"></a>

In this section, we handled data preprocessing tasks to prepare the dataset for analysis and modeling. Key steps include:

- Loading and examining the dataset.
- Handling missing values.
- Performing one-hot encoding on categorical features.
- Isolating the outcome variable (attrition) and selecting the features.

## 3. Exploratory Data Analysis (EDA) <a name="exploratory-data-analysis"></a>

Exploratory Data Analysis (EDA) helps us understand the dataset and identify factors contributing to employee attrition. The following analyses were performed:

- Descriptive statistics to understand data distributions.
- Visualization using various plots and charts to uncover patterns and relationships.
- Identification of potential features that could impact attrition, such as employee satisfaction levels.

## 4. Model Building and Evaluation <a name="model-building-and-evaluation"></a>

In this stage, we built and evaluated machine learning models to predict employee attrition. Key components include:

- Splitting the data into training and testing sets.
- Implementing two types of models: Logistic Regression, Decision Tree, and Random Forest.
- Conducting grid search to find the best hyperparameters.
- Evaluating models using multiple scoring metrics like accuracy, precision, recall, F1, and ROC AUC.
- Extracting model evaluation metrics and presenting them in tabular format.

## 5. Feature Engineering <a name="feature-engineering"></a>

Feature engineering aimed to enhance model performance and mitigate data leakage. Actions taken include:

- Excluding the 'satisfaction_level' feature.
- Creating a new binary feature called 'overworked' to capture employee overwork.
- Dropping the 'average_monthly_hours' feature.

## 6. Conclusion and Recommendations <a name="conclusion-and-recommendations"></a>

**Conclusion:**

- The logistic regression model achieved a precision of 80%, recall of 83%, and an F1-score of 80%.
- The decision tree model, after feature engineering, achieved an AUC of 93.8%, precision of 87.0%, recall of 90.4%, and an F1-score of 88.7%.
- The random forest model outperformed the decision tree model, especially in terms of AUC (94%).

**Recommendations:**

- Implement a cap on the number of projects employees can work on to prevent excessive workload.
- Recognize and promote employees with at least four years of tenure.
- Ensure fair compensation or incentives for employees working longer hours.
- Communicate overtime pay policies and clarify workload and time-off expectations.
- Conduct cultural evaluations and initiate improvements.
- Review the evaluation score system for fairness.

## 7. Next Steps <a name="next-steps"></a>

Moving forward, consider the following next steps:

- Evaluate how model predictions change when the 'last_evaluation' feature is removed from the data to assess data leakage.
- Explore the use of K-Means clustering analysis to analyze employee clusters.
- Implement the recommended actions to address workforce challenges and improve employee retention.

This project provides valuable insights into the factors affecting employee attrition and suggests actionable steps for enhancing the work environment and reducing attrition rates.

## Recommendations
This project concludes that employee overwork is a significant issue requiring HR intervention. Recommendations include capping project assignments, recognizing and promoting tenured employees, ensuring fair workload and overtime compensation, clarifying policies and expectations, conducting cultural evaluations, and reviewing performance reward scaling. Future steps include evaluating data leakage from the last evaluation feature and exploring k-means clustering to analyze employee clusters.
To retain employees and create a healthier work environment, consider the following recommendations for stakeholders:

- Cap Project Assignments: Implement a limit on the number of projects employees can work on simultaneously to prevent excessive workload.
- Tenure-Based Recognition: Recognize and promote employees who have been with the company for at least four years, and investigate the reasons behind the dissatisfaction of four-year tenured employees.
- Fair Workload and Overtime: Ensure fair compensation or incentives for employees working longer hours, or reconsider workload expectations.
- Communication and Policy Clarity: Inform employees about overtime pay policies, and clarify expectations regarding workload and time-off.
- Cultural Evaluation: Conduct company-wide and team-specific discussions to understand and address the work culture, seeking improvements in various contexts.
- Performance Reward Scaling: Review the evaluation score system to ensure that high scores are not reserved solely for employees working 200+ hours per month. Consider a proportionate scale for rewarding effort and contributions.

## Next Steps

While addressing the identified issues, consider the following next steps:

- Data Leakage Evaluation: Assess how predictions change when the 'last_evaluation' feature is removed from the data. Determine whether it's essential for predicting employee retention or whether other factors, such as performance or satisfaction scores, can be more informative.
- K-Means Analysis: For future projects, explore the use of a K-Means clustering model on this data to analyze employee clusters. This analysis may yield valuable insights into employee groups and their characteristics.

These actions and next steps aim to improve employee retention, foster a healthier work environment, and ensure data-driven decision-making in addressing workforce challenges.

## Key Stats
- Mercedes-Benz Group had **172,425** employees in **2021**, with **36%** women and **56%** white employees.
- The company also employed **4,817** trainees and **9,531** employees in its mobility division.
- The company's HR strategy focuses on three pillars: Re-Shape, Re-Skill, and Re-Charge, with an aim to be an attractive employer by fostering a culture of trust.

References:
- [Key figures Human Resources - Mercedes-Benz Sustainability Report 2021](https://sustainabilityreport.mercedes-benz.com/2021/appendix/key-figures/key-figures-human-resources.html)
- [HR work in the transformation - Mercedes-Benz Group Sustainability](https://sustainabilityreport.mercedes-benz.com/2022/social/people/hr-work-in-the-transformation.html)
- [How Mercedes Benz UK uses workforce analytics in resourcing](https://www.haystalentsolutions.com/-/how-mercedes-benz-uk-uses-workforce-analytics-in-resourcing)
- [Mercedes-Benz USA demographics and statistics - Zippia](https://www.zippia.com/mercedes-benz-usa-careers-31064/demographics/)


