Assignment 1 - Churn Rate Analysis
Project Title
DAI Assignment 1 - Churn Rate Analysis

Author
23112043 - Ishan Tandon


Project Overview
This project focuses on analyzing the churn rate of a company by examining customer data. The project involves cleaning, analyzing, and visualizing the data to draw meaningful conclusions regarding the company's customer retention patterns.

Objectives:

Clean the raw dataset for analysis.

Perform univariate and bivariate analysis.

Group the data into relevant columns for better insights.

Analyze the key factors contributing to customer churn.

Draw conclusions based on the analysis.


Workflow
1. Data Cleaning
Handled missing or inconsistent values in the dataset.
Removed irrelevant columns that don't contribute to the analysis.
2. Data Grouping
Grouped customers based on their tenure and payment methods.
3. Univariate Analysis
Analyzed individual columns (e.g., tenure, payment methods) to understand distributions.
4. Bivariate Analysis
Performed analysis between different pairs of columns to understand relationships (e.g., payment method vs. churn rate, tenure vs. churn).
5. Conclusion
Summarized findings from the analysis, highlighting the key factors influencing customer churn.

Technologies Used
Python (Pandas, Matplotlib, Seaborn)
Jupyter Notebook

Conclusion

Based on the analysis, several factors such as payment methods, tenure, and internet service usage were found to significantly impact the churn rate. These insights can help the company improve its customer retention strategies.


**Assignment-2**



**Data Analysis and Regression with Tips Dataset**

This project demonstrates a data analysis and regression workflow on a dataset containing information on restaurant tips. The analysis involves data loading, cleaning, exploratory data analysis (EDA), and setting up a regression model to predict outcomes based on the dataset features.

**Project Structure**

Jupyter Notebook:
The main file, DAI_2_23112043.ipynb, contains the code and documentation for the data analysis and regression tasks.
Dataset: The notebook loads a dataset named tips (data for regression problem) (1).csv, which should be placed in the appropriate directory if you’re running the notebook locally.

Requirements
To run this notebook, you need the following Python libraries:

pandas
numpy
matplotlib
seaborn
scikit-learn


**Steps Covered in the Notebook**
Data Loading and Preprocessing:
You began by uploading the dataset (using screenshots of code or relevant parts) and performing initial data exploration. This likely involved checking for missing values, understanding data types, and getting familiar with the variables.
Exploratory Data Analysis (EDA) Using Pair Plot:

1.You used a pair plot to visualize the relationships between different numerical variables, with color coding for categorical variables like "smoker."
The pair plot provided insights into the correlation patterns, distribution of variables, and possible group differences (e.g., how "smoker" affects the "tip" or "total_bill").

2.Linearity Check Using the Rainbow Test:
You applied the Rainbow Test to check if there was linearity between the dependent variable (like "tip" or "total_bill") and other independent variables.
The Rainbow Test helps determine if a linear model is suitable for the data by testing for a linear relationship, allowing you to confirm or reject linearity assumptions.

3.Correlation Analysis with a Heatmap:
You used a heatmap to analyze the correlations between numerical variables.
The heatmap provided a visual representation of the correlation coefficients, helping identify highly correlated variables. This information is useful in understanding which variables might have a strong influence on the target variable or could cause multicollinearity issues in regression models.

4.Applying Various Regression Models:
You applied multiple regression models, including:
Linear Regression (basic regression model),
Ridge Regression and Lasso Regression (regularized linear models),
Decision Tree Regression and Random Forest Regression (tree-based models),
Support Vector Regression (using different kernels), and
K-Nearest Neighbors Regression.

For each model, you trained it on the data and evaluated its performance using the R² score on the test set. The R² score measures how well the model explains the variance in the target variable.

5.Selecting the Model with the Highest R² Score:
After evaluating all models, you identified the model with the highest R² score, indicating it had the best predictive performance on the test data.

6.Hyperparameter Tuning Using Grid Search CV:
To further improve model performance, you fine-tuned the model with the highest R² score using GridSearchCV, a cross-validation-based hyperparameter tuning method.
GridSearchCV systematically tested combinations of hyperparameters to find the optimal configuration for each model.
After tuning, you re-evaluated the best model on the test data to confirm that the optimized parameters improved the R² score.

Summary of Optimized Results:
You compiled the final results into a DataFrame, showing the best hyperparameters and R² scores for each model.
This allowed for easy comparison and provided a comprehensive view of model performance, from initial trials to fine-tuned versions.


Usage
To run the notebook:

Clone the repository.
Ensure the dataset is in the specified path within the notebook.
Run the cells sequentially to reproduce the analysis and model results.
Results
The final section of the notebook provides insights from the regression model and visualizations to interpret the model's predictions.
