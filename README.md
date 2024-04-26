# Gun Violence Incident Fatality Predictor

This project aims to predict the fatality of gun violence incidents based on data collected from various police departments across the United States.

## Original Dataset

The original dataset used in this project was preprocessed by the group. It comprised data from 22 Police Departments, with a focus on four main departments: Baltimore PD, Boston PD, Los Angeles PD, and San Francisco PD. The dataset contained a total of 162,470 rows and 17 columns.

**Data Selection Criteria:**
1. All departments had 'Non-Fatal Shooting' and 'Homicide-Gun' variables under the 'offence_group' column, except for Los Angeles PD.
2. Los Angeles PD had 'Homicide-Criminal-Fatal-Shooting' and 'Agg Assault - Shooting - Non-Fatal' under the 'offence_category' column.

**Note:** Newark PD was dropped from the analysis due to a high percentage of missing values in crucial columns.

The group performed the following preprocessing steps on the original dataset:
- Loaded the dataset and performed an initial exploration.
- Cleaned the data by handling missing values, duplicates, and irrelevant columns.
- Categorized variables such as victim age, sex, race, season, and time of day for analysis.
- Created categorical variables for victim age, sex, race, season, and time of day.
- Performed one-hot encoding for categorical variables.

## Modified Dataset

The modified dataset is the result of applying Python code to further process the preprocessed data. The modifications include:
- Consolidating certain categories within variables (e.g., consolidating various weapon types into broader categories).
- Removing non-gun crimes from the dataset.
- Dropping redundant columns.
- Encoding binary variables.
- Conducting additional feature engineering (e.g., categorizing time into buckets).

After these modifications, the dataset is ready for modeling. The cleaned dataset contains [insert number of rows] rows and [insert number of columns] columns.

The machine learning model reads the cleaned dataset, which includes all the necessary features and target variable ('fatality_status') for training and prediction purposes.

## Conclusion

The Gun Violence Incident Fatality Predictor project involves preprocessing an original dataset provided by the group and making necessary modifications using Python code to prepare it for modeling. By following these steps, the dataset becomes suitable for training and evaluating machine learning models to predict the fatality of gun violence incidents.
