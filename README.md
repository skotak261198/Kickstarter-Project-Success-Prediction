# Kickstarter Project Success Prediction

## Overview

This project focuses on exploring and cleaning data, developing machine learning models, and making predictions to determine the success of crowdfunding projects on Kickstarter.com. The goal is to accurately predict whether a Kickstarter project will achieve its fundraising goal based on various features, using logistic regression and tree-based models.

## Problem Statement

Kickstarter.com is a crowdfunding platform where projects must reach or exceed a user-specified funding goal to be considered successful. If the goal is met, the project creator receives all the funds raised; if not, they receive nothing. This project aims to predict the binary outcome of project success ("YES" if successful, "NO" otherwise) using machine learning techniques on a set of provided data.

## Data Description

The dataset includes information on over 100,000 Kickstarter projects with deadlines from 2009 to 2014. We are provided with approximately 60 features for each project to analyze and build predictive models. The data is divided into multiple CSV files for training and testing:

- **ks_training_X.csv**: Features for training instances (projects with deadlines before September 2014).
- **ks_training_y.csv**: Labels for the target variables corresponding to the training instances.
- **ks_test_X.csv**: Features for test instances (projects with deadlines from September to December 2014). The objective is to make predictions for these instances.
- **small_training_X.csv**: A smaller subset of the training features (10,000 instances) for quicker data exploration in R.
- **small_training_y.csv**: Corresponding labels for the smaller training set.
- **ks_test_y_FAKE.csv**: A fake set of labels for the test set (all "NO") to simplify coding and testing.

## Project Objectives

1. **Data Exploration and Preprocessing**:
   - Perform exploratory data analysis (EDA) to understand the dataset's structure and identify patterns.
   - Preprocess the data by handling missing values, encoding categorical variables, and normalizing features as needed.

2. **Model Development**:
   - Develop logistic regression and tree-based models to classify projects as "successful" or "unsuccessful."
   - Utilize the training dataset to train the models and fine-tune hyperparameters for optimal performance.

3. **Model Evaluation and Interpretation**:
   - Evaluate the models using appropriate metrics such as accuracy, precision, recall, F1-score, and AUC-ROC to measure their performance.
   - Interpret the model results to understand the factors contributing most significantly to project success.

4. **Prediction on Test Set**:
   - Apply the trained models to the test dataset (ks_test_X.csv) to predict the likelihood of project success.
   - Assess the generalization of the models to unseen data.

## Methodology

1. **Data Preparation**:
   - Read and preprocess the data to handle missing values and ensure all features are suitable for model input.
   - Conduct EDA to visualize key relationships and distribution of features.

2. **Feature Engineering**:
   - Derive new features if needed to enhance model performance.
   - Transform categorical features using encoding techniques and normalize numerical features.

3. **Model Building**:
   - Train logistic regression models to predict project success probability.
   - Develop decision tree and ensemble-based models (like Random Forests) to capture non-linear relationships in the data.

4. **Model Tuning and Selection**:
   - Perform hyperparameter tuning using cross-validation to optimize model performance.
   - Select the best-performing model based on validation metrics.

5. **Prediction and Evaluation**:
   - Make predictions on the test dataset and evaluate the models using a comprehensive set of performance metrics.
   - Analyze and interpret the outcomes to draw meaningful conclusions about Kickstarter project success factors.

## Deliverables

- A well-formatted HTML report generated using R Markdown, including:
  - Clear answers to the assignment questions.
  - Relevant plots and tables to illustrate data insights and model performance.
  - Embedded R code demonstrating the data analysis process and model development steps.

## How to Run the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/kickstarter-success-prediction.git
   cd kickstarter-success-prediction
