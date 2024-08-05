# Stroke Prediction Machine Learning Project

## Project Overview

This repository contains the code and documentation for a machine learning project focused on predicting the likelihood of stroke occurrence based on various health and lifestyle factors. The project utilizes multiple supervised and unsupervised learning algorithms to analyze a dataset of patient information and predict stroke risk.

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Problem Statements](#problem-statements)
4. [Data Exploration and Preprocessing](#data-exploration-and-preprocessing)
5. [Data Visualization](#data-visualization)
6. [Model Development](#model-development)
7. [Results](#results)

## Introduction

Stroke is a leading cause of death worldwide, with an estimated 17.9 million deaths annually due to cardiovascular diseases. This project aims to leverage machine learning techniques to predict stroke risk based on various factors such as age, gender, health conditions, and lifestyle choices. By accurately predicting stroke risk, we can potentially assist healthcare providers in early intervention and prevention strategies.

## Dataset Description

The dataset used in this project is sourced from Kaggle and contains the following features:

- id: Unique identifier
- gender: "Male", "Female" or "Other"
- age: Age of the patient
- hypertension: 0 (doesn't have hypertension) or 1 (has hypertension)
- heart_disease: 0 (doesn't have heart disease) or 1 (has heart disease)
- ever_married: "No" or "Yes"
- work_type: "children", "Govt_job", "Never_worked", "Private" or "Self-employed"
- Residence_type: "Rural" or "Urban"
- avg_glucose_level: Average glucose level in blood
- bmi: Body Mass Index
- smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"
- stroke: 0 (no stroke) or 1 (had stroke)

The dataset contains 5110 observations with both categorical and numerical data.

## Problem Statements

This project addresses the following key questions:

1. How can one predict a stroke based on the other attributes?
2. What other factors can be used to predict heart disease?
3. Does the nature of work cause somebody to have heart disease?
4. Based on the glucose level, which age group and worker type has a higher risk of heart disease?

## Data Exploration and Preprocessing

The data exploration and preprocessing phase included:

1. Examining the dataset structure and summary statistics
2. Handling missing values (particularly in the BMI column)
3. Encoding categorical variables
4. Dropping unnecessary columns
5. Scaling numerical features

## Data Visualization

Various visualization techniques were employed to gain insights into the data:

1. Bar plots to show the relationship between categorical variables and stroke occurrence
2. Scatter plots to visualize the relationship between age, glucose levels, and stroke risk
3. Joint plots to combine univariate and bivariate analyses

Key visualizations include:
- Gender vs. Stroke occurrence
- Age vs. Stroke occurrence
- Work Type vs. Stroke occurrence
- Residence Type vs. Stroke occurrence
- Age vs. Average Glucose Level (with stroke indication)

## Model Development

The project implements several machine learning algorithms:

### Supervised Learning
1. Random Forest
2. Decision Tree
3. Logistic Regression

### Unsupervised Learning
1. K-Means Clustering

Each algorithm was implemented using the scikit-learn library in Python. The data was split into training and testing sets to evaluate model performance.

## Results

Model performance for stroke prediction:

1. Random Forest: 
   - Train accuracy: 100%
   - Test accuracy: 94.1%

2. Logistic Regression:
   - Test accuracy: 78.0%

3. Decision Tree:
   - Train accuracy: 76.628%
   - Test accuracy: 76.38%

For heart disease prediction:

1. Random Forest:
   - Train accuracy: 100%
   - Test accuracy: 94%

2. Logistic Regression:
   - Test accuracy: 82.0%

3. Decision Tree:
   - Train accuracy: 79.51%
   - Test accuracy: 79.25%

The K-Means clustering algorithm was used for unsupervised learning to identify patterns in the data without predefined labels.

## Conclusion

The Random Forest algorithm demonstrated the highest accuracy (94.1%) in predicting stroke risk. This model can be used to assist in early detection and prevention of strokes by identifying high-risk individuals based on their health and lifestyle factors.
