# Logistic Rgression vs Decision Trees


In this project, I compare Logistic Regression and Decision Tree Classifiers on a binary classification problem using a small, real-world dataset. The goal is to evaluate how both models perform under realistic conditions involving:
- Multiple categorical features
- Missing values requiring imputation or handling
- A relatively imbalanced target variable
- The need for proper data preprocessing and feature engineering

## Why This Dataset?
This dataset was intentionally selected to demonstrate the ability to work with imperfect, real-world data. It presents several common challenges, including:
- Missing values
- Categorical features
- Class imbalance
- Limited sample size

Rather than discarding problematic records, the focus was on applying effective preprocessing techniques to retain as much valuable data as possible. This project provides a practical setting to evaluate model performance in a binary classification task, highlighting the differences between Logistic Regression and Decision Tree models when applied to noisy, small-scale data.

## Model Comparison Rationale
While Logistic Regression is widely regarded as a strong baseline for binary classification tasks, and Decision Trees are often recommended for handling more complex, multiclass problems, I set out to empirically evaluate these assumptions.

## Project Overview
- This project demonstrates a complete binary classification pipeline using both Logistic Regression and Decision Tree models, with a strong focus on data preprocessing, model evaluation, and reproducibility.

## Data Preprocessing
Robust preprocessing techniques are applied, including:
- Handling missing values with appropriate imputation strategies
- Encoding categorical variables while maintaining interpretability
- Emphasis on preserving data quality and minimizing information loss

## Analytical Approach
- The project reflects a careful and analytical mindset, exploring model performance on a small, real-world dataset. Considerations around bias-variance trade-off, model complexity, and generalizability are explicitly addressed.

## Python & Code Quality
- Clean, modular, and well-documented code
- Comments are used generously to enhance clarity and learning value
- Code readability and transparency are prioritized throughout

## Model Serialization
- The Logistic Regression model is serialized using Pickle, demonstrating how to:
- Save a trained model to disk
- Reload it to perform inference on new or unseen data
- This highlights a foundational aspect of deploying ML models in real-world applications.

##  Hyperparameter Optimization
- For the Decision Tree classifier, GridSearchCV is employed to fine-tune model parameters, ensuring optimal performance. The process includes:
- Cross-validation to guard against overfitting
- Selection of the best model based on scoring metrics

## The project is organized into the following sections:

- **Dataset Preprocessing:** Initial data cleaning, handling missing values, and encoding categorical variables.
  - [Pre-Processing](pre-processing-dataset.ipynb)   

- **Preprocessing & Logistic Regression Model:** Building and evaluating a Logistic Regression model using the preprocessed data.
  - [Logistic Regression model](Pre-Processing_Logistic_Regression_model.ipynb)

- **Preprocessing & Decision Tree Model:** Building and tuning a Decision Tree model, including hyperparameter optimization using GridSearchCV.
  - [Decision Tree model](Pre-Processing-Decision_Tree_Model.ipynb)
 
## Key Findings & Reflections
- Given the limited size of the dataset, I anticipated that drawing a clear performance distinction between the two models might be challenging. Nonetheless, the results provided meaningful insights:
- Logistic Regression outperformed the Decision Tree on the test set, achieving an accuracy of 86%.
- Both models delivered reasonable performance, particularly considering the dataset's small size and imperfections.
- From a practical standpoint, I continue to favor Logistic Regression for binary classification tasks involving structured, tabular data—especially when working with smaller datasets. Its simplicity, interpretability, and reliable generalization make it a strong and 
  dependable baseline in many applied machine learning workflows.
