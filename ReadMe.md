# Movie Rating Prediction

This project focuses on predicting movie ratings based on a dataset consisting of movie information and user ratings. The dataset is composed of three main files: `movies.dat`, `ratings.dat`, and `users.dat`. The project involves performing Exploratory Data Analysis (EDA), data preprocessing, and building a regression model for predicting movie ratings.

## Dataset Overview

The dataset comprises the following files:

1. `movies.dat`: Contains information about movies, including movie IDs, titles, and genres.
2. `ratings.dat`: Contains user ratings for movies, including user IDs, movie IDs, ratings, and timestamps.
3. `users.dat`: Contains user information, including user IDs, gender, age, occupation, and zip codes.

## Exploratory Data Analysis (EDA)

EDA is conducted on each dataset file to gain insights and understand the data.

### Movies Dataset

The movies dataset is loaded and the following exploratory steps are performed:

- Displaying the first few rows of the dataset.
- Checking the dataset's information, including column names and data types.
- Describing the dataset to obtain summary statistics.
- Visualizing the distribution of movie genres using a bar plot.
- Analyzing the distribution of movie title lengths using a histogram.
- Analyzing the number of movies released each year using a line plot.

### Ratings Dataset

The ratings dataset is loaded and the following exploratory steps are performed:

- Displaying the first few rows of the dataset.
- Checking the dataset's information, including column names and data types.
- Describing the dataset to obtain summary statistics.
- Visualizing the distribution of ratings using a histogram.
- Analyzing the distribution of the number of ratings per user using a histogram.
- Analyzing the distribution of the number of ratings per movie using a histogram.

### Users Dataset

The users dataset is loaded and the following exploratory steps are performed:

- Displaying the first few rows of the dataset.
- Checking the dataset's information, including column names and data types.
- Describing the dataset to obtain summary statistics.
- Visualizing the distribution of age using a histogram.
- Analyzing the gender distribution using a bar plot.
- Analyzing the occupation distribution using a bar plot.

## Data Preprocessing

After performing EDA, data preprocessing steps are carried out to prepare the data for modeling. The following preprocessing steps are applied:

- Encoding categorical variables: The gender column in the users dataset is encoded as 0 for Female and 1 for Male using label encoding.
- Merging datasets: The movies, ratings, and users datasets are merged based on common columns.
- Handling missing values: Any missing values in the dataset are identified and handled appropriately.

## Regression Model for Movie Rating Prediction

A regression model is built using the XGBoost algorithm to predict movie ratings. The following steps are performed:

- Sample selection: A 20% random sample of the merged dataset is selected for modeling.
- Splitting the data: The dataset is split into features (X) and the target variable (y).
- Training the model: An XGBoost regression model is trained on the training data.
- Making predictions: The trained model is used to make predictions on the test data.
- Evaluating the model: The Mean Squared Error (MSE) is calculated to evaluate the model's performance.
- Visualizing the predicted vs. actual ratings using a scatter plot.
- Visualizing the feature importance using a bar plot.

## Movie Rating Prediction on Test Data

A test dataset is created to demonstrate the movie rating prediction. The dataset contains various features related to the movie, such as gender, age, year, genre, and title encoded. The trained XGBoost regression model is used to predict the ratings for the test data.

## Conclusion

This project showcases the process of predicting movie ratings using machine learning techniques. By exploring and preprocessing the data, building a regression model, and evaluating its performance, we can gain insights into the factors influencing movie ratings and develop a powerful model for predicting ratings. The project highlights the importance of data analysis, preprocessing, and model selection in making accurate predictions in the movie rating domain.