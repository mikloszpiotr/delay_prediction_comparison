# Delay Prediction Model Comparison

This repository contains a Jupyter notebook that compares **classification** models for predicting delay risk in logistics, transportation, or similar operations.

The goal is to provide a structured, business-oriented benchmark of multiple machine learning models using both technical metrics and cost-based evaluation.

---

## Project Overview

The notebook walks through the end-to-end process: generating a realistic synthetic logistics dataset, exploring it, engineering features, training several classifiers, and analyzing their performance. 
It is designed for analytics and supply chain practitioners who want to understand which model balances accuracy, recall, and business cost in delay prediction problems.

---

## Scenario and Data

The dataset simulates delivery or transport operations with around 2,000 observations.

- **Features** include Distance, Time_of_Day, Day_of_Week, Weather, Traffic, and Priority level.
- **Target** is Delay_Status: 0 (On-Time) or 1 (Delayed), with an additional human-readable Delay_Label.

---

## Implemented Models

The notebook trains and compares several classification models using a common pipeline.

- **Logistic Regression**.
- **Decision Tree**.
- **Random Forest**.
- **Gradient Boosting**.
- **Support Vector Machine (SVM)**.
- **K-Nearest Neighbors (KNN)**.
- **Neural Network** (MLPClassifier).

Each model is evaluated using accuracy, precision, recall, F1 score, and AUC, plus confusion matrices and ROC/PR curves.

---

## Business Cost Analysis

Beyond pure ML metrics, the notebook includes a **cost-based** evaluation that assigns different penalties to false negatives and false positives.

A summary table reports, for each model: total cost, number of false negatives, and number of false positives to support informed business decisions.

---

## Repository Structure

```text
.
├── delay_prediction_comparison.ipynb  # Main notebook with full workflow
└── README.md                          # Project description and usage
