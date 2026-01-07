# Delay Prediction Model Comparison

This repository contains a Jupyter notebook that compares **classification** models for predicting delay risk in logistics, transportation, or similar operations. [file:2]

The goal is to provide a structured, business-oriented benchmark of multiple machine learning models using both technical metrics and cost-based evaluation. [file:2]

---

## Project Overview

The notebook walks through the end-to-end process: generating a realistic synthetic logistics dataset, exploring it, engineering features, training several classifiers, and analyzing their performance. [file:2]

It is designed for analytics and supply chain practitioners who want to understand which model balances accuracy, recall, and business cost in delay prediction problems. [file:2]

---

## Scenario and Data

The dataset simulates delivery or transport operations with around 2,000 observations. [file:2]

- **Features** include Distance, Time_of_Day, Day_of_Week, Weather, Traffic, and Priority level. [file:2]  
- **Target** is Delay_Status: 0 (On-Time) or 1 (Delayed), with an additional human-readable Delay_Label. [file:2]  

---

## Implemented Models

The notebook trains and compares several classification models using a common pipeline. [file:2]

- **Logistic Regression**. [file:2]  
- **Decision Tree**. [file:2]  
- **Random Forest**. [file:2]  
- **Gradient Boosting**. [file:2]  
- **Support Vector Machine (SVM)**. [file:2]  
- **K-Nearest Neighbors (KNN)**. [file:2]  
- **Neural Network** (MLPClassifier). [file:2]  

Each model is evaluated using accuracy, precision, recall, F1 score, and AUC, plus confusion matrices and ROC/PR curves. [file:2]

---

## Business Cost Analysis

Beyond pure ML metrics, the notebook includes a **cost-based** evaluation that assigns different penalties to false negatives and false positives. [file:2]

A summary table reports, for each model: total cost, number of false negatives, and number of false positives to support informed business decisions. [file:2]

---

## Repository Structure

```text
.
├── delay_prediction_comparison.ipynb  # Main notebook with full workflow
└── README.md                          # Project description and usage
