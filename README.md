Gun Violence Incident Fatality Predictor
This project aims to predict the fatality of gun violence incidents based on data collected from various police departments across the United States.

Dataset
The dataset used in this project consists of data from 22 Police Departments, with a focus on four main departments:

Baltimore PD
Boston PD
Los Angeles PD
San Francisco PD
The dataset contains a total of 162,470 rows and 17 columns.

Data Selection Criteria:

All departments have 'Non-Fatal Shooting' and 'Homicide-Gun' variables under the 'offence_group' column, except for Los Angeles PD.
Los Angeles PD has 'Homicide-Criminal-Fatal-Shooting' and 'Agg Assault - Shooting - Non-Fatal' under the 'offence_category' column.
Note: Newark PD was dropped from the analysis due to a high percentage of missing values in crucial columns.

Data Preprocessing
Loaded the dataset and performed an initial exploration.
Cleaned the data by handling missing values, duplicates, and irrelevant columns.
Categorized variables such as victim age, sex, race, season, and time of day for analysis.
Feature Engineering
Created categorical variables for victim age, sex, race, season, and time of day.
Performed one-hot encoding for categorical variables.
Transformed the dataset for modeling.
Model Building
Decision Tree Classifier
Utilized a Decision Tree Classifier with a maximum depth of 10.
Achieved an accuracy of [insert accuracy here].
Logistic Regression
Implemented Logistic Regression with the 'liblinear' solver.
Achieved an accuracy of [insert accuracy here].
Random Forest Classifier
Conducted a grid search to optimize hyperparameters.
Achieved the best accuracy of [insert best accuracy here] with the following parameters: [insert best parameters here].
Evaluation
Evaluated models using confusion matrices, accuracy scores, and classification reports.
Visualized ROC curves and calculated Youden's J statistic.
Conclusion
The Gun Violence Incident Fatality Predictor demonstrates the potential of machine learning models in predicting the outcome of gun violence incidents. Further improvements and optimizations can be made to enhance the model's performance and applicability.
