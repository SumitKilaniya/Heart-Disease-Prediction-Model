# Heart-Disease-Prediction-Model
Heart Disease Prediction: Exploratory Data Analysis (EDA)
This project contains the initial steps of a machine learning workflow, focusing on Exploratory Data Analysis (EDA) and data preprocessing for a heart disease prediction dataset. The goal is to understand the structure, quality, and statistical properties of the data before building a predictive model.

📁 Dataset
The analysis is based on the dataset: heart_disease_dataset.csv. The dataset contains 1000 records across 16 features (15 after preprocessing).

Key Features:
Heart Disease (int64): The target variable. (0 = No Disease, 1 = Disease)

Age (int64): Age of the individual.

Gender (object): Biological sex of the individual.

Cholesterol (int64): Cholesterol level.

Blood Pressure (int64): Blood pressure measurement.

Heart Rate (int64): Resting heart rate.

Smoking (object): Smoking status (Never, Current, Former).

Exercise Hours (int64): Weekly exercise hours.

Family History (object): History of heart disease in the family.

Diabetes (object): Diabetes status.

Obesity (object): Obesity status.

Stress Level (int64): Stress level score (1 to 10).

Blood Sugar (int64): Blood sugar level.

Exercise Induced Angina (object): Presence of exercise-induced angina.

Chest Pain Type (object): Type of chest pain (e.g., Typical Angina, Asymptomatic).

(Note: The Alcohol Intake column was dropped during the preprocessing stage.)

📈 Analysis & Preprocessing Steps
The primary steps executed in the notebook are:

1. Data Loading and Initial Inspection
Data was loaded using pandas.

Verified the dimensions of the dataset (1000 rows, 16 columns initially).

Checked data types and memory usage using data.info().

2. Handling Missing Values
Identified missing values exclusively in the Alcohol Intake column (340 null values, 34% of the data).

Attempts to impute the column with the mode (Heavy) were performed but failed due to a re-indexing issue.

Action Taken: The Alcohol Intake column was dropped from the dataset for the subsequent analysis.

3. Exploratory Data Analysis (EDA)
Univariate Analysis: Explored the distribution of categorical features, notably Smoking, showing that the three categories (Never, Current, Former) are almost equally represented.

Bivariate Analysis: A bar plot was generated to examine the relationship between Age and the target variable Heart Disease.

4. Feature Preprocessing Setup
The final step was setting up the LabelEncoder from sklearn for future encoding of the remaining object/categorical columns, preparing the data for model building.

🛠️ Requirements
The analysis was performed using the following Python libraries:

pandas

numpy

matplotlib.pyplot

seaborn

sklearn (specifically LabelEncoder)
