Rainfall Prediction in Australia using Machine Learning
This repository contains a data science project focused on predicting whether it will rain the next day in Australia. It demonstrates an end-to-end machine learning workflow, including data preprocessing, training multiple models, and comparative evaluation to identify the most effective algorithm for the task.

Project Overview:-
The primary objective of this project is to build and evaluate several supervised learning models for a binary classification problem: forecasting next-day rainfall. The analysis is performed on a historical weather dataset from various locations in Australia.

The project follows these key steps:

Data Loading and Preprocessing: Cleaning the data and transforming it into a format suitable for machine learning models.
Model Training: Implementing five different machine learning algorithms using the scikit-learn library.
Performance Evaluation: Assessing the models using various statistical metrics to compare their predictive power.
Reporting: Summarizing the results to identify the best-performing model.

Dataset:-
The project uses the Weather_Data.csv dataset, which contains daily weather observations from 2008 to 2017 across Australia.

Data Preprocessing
One-Hot Encoding: Categorical features such as RainToday, WindGustDir, WindDir9am, and WindDir3pm were converted into a numerical format.
Target Variable Transformation: The RainTomorrow column was converted from 'Yes'/'No' to a binary format (1/0).
Data Type Conversion: All feature columns were cast to the float data type to ensure consistency for modeling.

Methodology:-
Models Implemented
Five different models were trained and evaluated to find the best fit for the prediction task.

Linear Regression: Used to establish a baseline and evaluated with regression metrics.
K-Nearest Neighbors (KNN): A classifier was trained with the number of neighbors set to 4 (n_neighbors=4).
Decision Tree: A tree was built using the entropy criterion with a maximum depth of 4 (max_depth=4).
Logistic Regression: A model was trained using the liblinear solver.
Support Vector Machine (SVM): Implemented using the radial basis function (rbf) kernel.

Evaluation Metrics
The models were evaluated using the following metrics:

Classification: Accuracy Score, Jaccard Index, F1-Score, LogLoss.
Regression: Mean Absolute Error (MAE), Mean Squared Error (MSE), R2-Score.

Results:-
After training and evaluation, the performance of the classification models was compiled to identify the most effective algorithm. The Logistic Regression model demonstrated the strongest performance on the test data.
Here is a summary of the final scores for each model:

Logistic Regression (Top Performer):
Accuracy Score: 0.827481
Jaccard Index: 0.484018
F1-Score: 0.652308
LogLoss: 0.380085

Decision Tree:
Accuracy Score: 0.818321
Jaccard Index: 0.480349
F1-Score: 0.648968

K-Nearest Neighbors (KNN):
Accuracy Score: 0.818321
Jaccard Index: 0.425121
F1-Score: 0.596610

Support Vector Machine (SVM):
Accuracy Score: 0.722137
Jaccard Index: 0.000000
F1-Score: 0.000000

Technologies Used:-
Python
Pandas
NumPy

Scikit-learn

Jupyter Notebook
