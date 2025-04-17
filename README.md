# Logistic Rgression vs Decision Trees

In this project, I compare Logistic Regression and Decision Trees for a binary classification task using a small, real-world dataset. The dataset includes multiple categorical (object-type) features and contains missing values, making it a suitable challenge for evaluating model performance and data preprocessing strategies.

### Why This Dataset?
I selected this dataset to showcase my ability to handle imperfect data — particularly to preserve as much data as possible through effective preprocessing. My goal was to evaluate which model performs better on a small, imbalanced, and messy dataset within a binary classification context.

### Why These Models?
Logistic Regression is often cited as the go-to model for binary classification, while Decision Trees are frequently recommended for multiclass tasks. However, I wanted to put this theory to the test and explore how each model performs under the same conditions, using carefully tuned parameters and the same data preprocessing pipeline.

###  Project Overview
- **Data Preprocessing:** I demonstrate thorough preprocessing techniques, including handling missing values and encoding categorical features, with a focus on preserving as much of the original data as possible.

- **Analytical Thinking:** This project reflects my analytical mindset, as I explore model behavior and performance on a small dataset, carefully balancing complexity and generalizability.

- **Python Proficiency:** My code is clearly commented to demonstrate understanding — possibly a bit over-commented to ensure transparency 😄.

- **Model Serialization:** In the Logistic Regression section, I use Pickle to serialize and deserialize the trained model, showing how to save a model and reload it to make predictions on new data.

- **Hyperparameter Tuning:** For the Decision Tree model, I demonstrate the use of GridSearchCV to identify the optimal set of hyperparameters, ensuring the model is well-tuned for the dataset.

## The project is organized into the following sections:

- **Dataset Preprocessing:** Initial data cleaning, handling missing values, and encoding categorical variables.
  - [Pre-Processing](pre-processing-dataset.ipynb)   

- **Preprocessing & Logistic Regression Model:** Building and evaluating a Logistic Regression model using the preprocessed data.
  - [Logistic Regression model](Pre-Processing_Logistic_Regression_model.ipynb)

- **Preprocessing & Decision Tree Model:** Building and tuning a Decision Tree model, including hyperparameter optimization using GridSearchCV.
  - [Decision Tree model](Pre-Processing-Decision_Tree_Model.ipynb)
 
### Project Findings

Given the small size of the dataset, I anticipated it would be challenging to clearly demonstrate a definitive advantage for one model over the other.

However, Logistic Regression outperformed Decision Trees on the test set, achieving an accuracy of 86%, while both models performed reasonably well considering the limited data.

In my professional opinion, I prefer Logistic Regression for binary classification tasks due to its simplicity, interpretability, and consistent performance — especially on smaller datasets.
