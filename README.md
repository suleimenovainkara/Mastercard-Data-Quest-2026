# Hidden Entrepreneur Detection Using Transaction Data

## Overview

This project was developed for Mastercard Data Quest 2026 and focuses on identifying hidden commercial activity among individual bank cardholders.

Many self-employed individuals and small business owners conduct business transactions through personal consumer cards rather than dedicated business accounts. The goal of this project was to develop a machine learning framework capable of detecting such hidden entrepreneurs using transaction behavior data.

## Business Value

The solution enables financial institutions to:

- Identify potential business customers
- Increase revenue from acquiring and transaction services
- Improve targeting of business banking products
- Support cross-selling opportunities such as merchant acquiring, payroll services, and working capital financing

## Dataset

The project was based on anonymized transaction data provided within the Mastercard Data Quest competition.

The original datasets are not included in this repository due to data-sharing restrictions.

Datasets used:

- business_cards_mdq.parquet
- consumer_cards_mdq.parquet
- merchants_reference.parquet

## Methodology

A transaction-level feature engineering pipeline was developed to characterize customer behavior.

The following machine learning approaches were implemented and evaluated:

- Stacking Ensemble (LightGBM, XGBoost, CatBoost, Random Forest, Logistic Regression)
- Positive-Unlabeled (PU) Learning
- Isolation Forest
- One-Class SVM

## Results

The Stacking Ensemble model achieved the best overall performance.

Key outcomes:

- Multi-criteria score: 0.922
- Strong balance between predictive performance, business alignment, interpretability, and robustness

Risk segmentation results:

- High Priority: 3 cardholders
- Medium Priority: 9 cardholders
- Under Monitoring: 60 cardholders
- Not Suspicious: 79,928 cardholders

## Repository Structure

- code/ – feature engineering and model development
- presentation/ – competition presentation
- results/ – prediction outputs and visualizations

## Team Achievement

2nd Place — Mastercard Data Quest 2026

Role: Team Lead

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- LightGBM
- XGBoost
- CatBoost
- Random Forest
- Logistic Regression
- PU Learning
- Isolation Forest
- One-Class SVM
- K-means clustering
