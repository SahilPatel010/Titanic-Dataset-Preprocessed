Titanic Survival Data Analysis and Preprocessing
Project Overview
This project involves the comprehensive preprocessing and cleaning of the classic Titanic dataset. The primary objective is to transform the raw, messy passenger data into a clean, well-structured, and analysis-ready format. This foundational step is crucial for any future exploratory data analysis or for building a machine learning model to predict passenger survival.

The key tasks demonstrated in this project include handling missing values, creating dummy variables for categorical features, and performing feature engineering to extract meaningful information from complex columns.

Data Preprocessing Steps
The Jupyter Notebook in this repository (Titanic-Preprocessing.ipynb) details the following data cleaning and feature engineering steps:

Handling Categorical Data:

Pclass & Sex: Converted into numerical format using dummy variables to represent passenger class and gender.

Embarked: Filled missing values with the most common port of embarkation (the mode) and then converted the categories into dummy variables.

Handling Numerical Data:

Age: Filled a significant number of missing values using a strategic approach: imputing the mean age based on the passenger's class (Pclass). Infant ages (less than 1 year) were also handled by rounding to ensure data integrity.

Feature Engineering:

Cabin: Engineered a new, simpler Deck feature by extracting the first letter from the Cabin number. Missing values were consolidated into an 'Unknown' category, transforming a sparse and messy column into a useful feature.

Final Cleanup:

Dropped Unnecessary Columns: Removed columns like PassengerId, Name, Ticket, and the original Cabin column, as they were not useful for a quantitative analysis in their raw form.

Saved the Final Dataset: The final, clean DataFrame was saved to Titanic_preprocessedDataSet.csv.

How to Use This Repository
Clone the repository:

Bash

git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
Open the Jupyter Notebook:

Navigate to the project folder and open Titanic-Preprocessing.ipynb to see the full, step-by-step Python code.

View the Data:

Titanic-Dataset.csv is the original, raw data.

Titanic_preprocessedDataSet.csv is the final, clean dataset ready for analysis.

Tools and Libraries
Python 3

Pandas: For all data manipulation and cleaning.

NumPy: For numerical operations, particularly for rounding.

Jupyter Notebook: For interactive analysis and documentation.
