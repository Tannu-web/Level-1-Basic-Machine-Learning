# Level-1-Basic-Machine-Learning
This repository contains a Python script for a complete machine learning data preprocessing pipeline, covering missing data imputation, categorical feature encoding, numerical feature scaling, and dataset splitting.
Machine Learning Data Preprocessing Pipeline
This repository provides a foundational Python script for preprocessing raw datasets, a critical first step in any machine learning project. The code demonstrates a robust and reusable pipeline using pandas and scikit-learn to transform raw data into a clean, model-ready format.

Key Preprocessing Steps
The script systematically addresses the four core preprocessing tasks:

1. Handling Missing Data 🚮
Missing values in the dataset are handled using the SimpleImputer class. Numerical features are imputed with the mean value of their respective columns, while categorical features are filled with the most frequent value.

2. Encoding Categorical Variables 🏷️
Categorical data (like text-based features) is converted into a numerical format that machine learning models can understand. The script utilizes OneHotEncoder to create new binary columns for each unique category, which is a common practice for nominal data.

3. Normalizing Numerical Features 📈
Numerical features are standardized using StandardScaler. This process scales the data to have a mean of 0 and a standard deviation of 1. This is essential for algorithms that are sensitive to the scale of features, such as Support Vector Machines and K-Nearest Neighbors.

4. Splitting the Dataset ✂️
The dataset is split into training and testing sets using train_test_split. The training set is used to train a machine learning model, while the testing set is used to evaluate its performance on unseen data, ensuring an unbiased assessment.

How to Use
To use this script, simply follow these steps:

Replace the dataset: In the code, replace 'your_dataset.csv' with the path to your own dataset file.

Define features and target: Update the target_column variable to match the name of the column you want to predict.

Run the script: Execute the Python script. The output will show the shape of your preprocessed training and testing datasets, which are ready to be fed into a machine learning model.

Prerequisites
Python 3.x

pandas

scikit-learn

numpy
