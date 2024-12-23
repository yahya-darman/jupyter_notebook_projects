# Simple-Linear-Regression-Project
This repository contains data and code for a small linear regression project that aims to predict writing scores based on reading scores. The project uses a dataset that includes information about students' reading scores, writing scores, and other demographic information.

## Data
The [dataset](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams) used in this project is stored in the file StudentsPerformance.csv The file is a comma-separated value (CSV) file, with one row per student and the following columns:

- `gender`: the gender of the student (0 = female, 1 = male)
- `race/ethnicity`: the race/ethnicity of the student (group A to E)
- `parental level of education`: the highest level of education achieved by the student's parent(s)
- `lunch`: whether or not the student received free/reduced-price lunch (0 = standard, 1 = free/reduced)
- `test preparation course`: whether or not the student completed a test preparation course (0 = none, 1 = completed)
- `reading score`: the student's score on a reading exam (out of 100)
- `writing score`: the student's score on a writing exam (out of 100)
- `math score`: the student's score on a math exam (out of 100)

## Code
The code for the linear regression project is stored in the file Students_Performance.ipynb. The code performs the following steps:

1. Load the dataset from the `student_scores.csv` file using the Pandas library.
2. Split the dataset into input features (X) and the target variable (y), where X is the reading score column and y is the writing score column.
3. Split the data into training and testing sets using the `train_test_split()` function from the `sklearn.model_selection` module.
4. Fit a linear regression model on the training data using the `LinearRegression()` class from the `sklearn.linear_model` module.
5. Predict the values of the target variable (writing scores) using the fitted linear regression model and the testing input data (reading scores).
6. Compute the mean squared error and R^2 score of the linear regression model on the testing data using the `mean_squared_error()` and `r2_score()` functions from the `sklearn.metrics` module.
7. Plot a scatter plot of the actual writing scores vs the predicted writing scores.

## Results
The linear regression model achieved a mean squared error of 4.65 and an R^2 score of 0.90 on the testing data, indicating that the model is a good fit for the data. The scatter plot of the actual writing scores vs the predicted writing scores shows a clear positive correlation between the two variables, with the majority of the data points falling close to the line of best fit.

## Dependencies
This project requires the following dependencies:

- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Seaborn
