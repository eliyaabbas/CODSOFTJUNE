# Iris Flower Identification

This repository contains code for performing iris flower identification using the Iris dataset. It includes data preprocessing, exploratory data analysis (EDA), visualization plots, and training a Random Forest Classifier for prediction.

## Dataset

The Iris dataset is loaded from the 'iris_dataset.csv' file. It consists of measurements of sepal length, sepal width, petal length, petal width, and the corresponding species label.

## Exploratory Data Analysis (EDA)

EDA is performed to gain insights into the dataset. The following steps are performed:

- Display dataset overview using `iris_data.head()` to show the first few rows.
- Calculate and print data summary using `iris_data.describe()`.
- Visualize the relationship between sepal length and sepal width using a scatter plot.
- Visualize the relationship between petal length and petal width using a scatter plot.
- Visualize the distribution of each feature using box plots.

## Preprocessing

Data preprocessing steps include:

- Preparing the features and target variables.
- Encoding the target variable using `LabelEncoder`.

## Model Training and Evaluation

The Random Forest Classifier is trained on the preprocessed data using `train_test_split`. The model is evaluated using accuracy score on the test set.

## Prediction

The model is tested with new input data for prediction. An example input data is provided, and the predicted species is displayed.

## Requirements

The code requires the following libraries to be installed:

- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn

## Usage

1. Ensure the required libraries are installed.
2. Place the 'iris_dataset.csv' file in the same directory as the code file.
3. Run the code to perform EDA, visualize plots, train the model, and make predictions.

Feel free to customize the code and explore additional analyses or techniques as per your requirements.

