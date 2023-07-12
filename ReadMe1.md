# Titanic Survivor Prediction

This project focuses on predicting the survival of passengers aboard the Titanic using machine learning techniques. The dataset used for this analysis consists of information such as passenger details, ticket information, fare, and survival status.

## Libraries Used

The following libraries were utilized for this project:

- Pandas (imported as pd): Used for data manipulation and analysis.
- NumPy (imported as np): Used for numerical computations and array operations.
- Regular Expression (imported as re): Used for text pattern matching and extraction.
- Matplotlib.pyplot (imported as plt): Used for data visualization and creating plots.
- Train-Test Split from sklearn.model_selection: Used for splitting the data into training and testing sets.
- RandomForestClassifier from sklearn.ensemble: Used as the machine learning model for prediction.
- Accuracy Score from sklearn.metrics: Used for evaluating the accuracy of the model.
- MinMaxScaler from sklearn.preprocessing: Used for normalizing the numerical features.
- Preprocessing from sklearn: Used for label encoding categorical features.

## Data Processing and Modeling Steps

1. Data Loading: The training data is loaded from the 'train.csv' file into a DataFrame using pd.read_csv(). Similarly, the test data is loaded from the 'test.csv' file into a DataFrame called 'test_data1'.

2. Data Preprocessing:
   - Irrelevant features are dropped using the drop() method, including 'PassengerId', 'Name', and 'Cabin' columns.
   - The 'Ticket' column is converted from categorical to numerical by extracting ticket prefixes using regular expressions.
   - Missing values in the 'Age' column are filled with the median value, and the column is converted to the integer data type.
   - The 'Embarked' column is also filled with the mode (most frequent value) and mapped to numerical values.
   - Categorical features 'Sex' and 'Embarked' are converted to numerical using label encoding.

3. Data Normalization: The 'Fare' column is normalized using the MinMaxScaler from sklearn.preprocessing.

4. Training and Evaluation:
   - The feature matrix 'X' is created by dropping the 'Survived' and 'Fare' columns from the training data, and the target vector 'y' is set as the 'Survived' column.
   - The data is split into training and testing sets using train_test_split() from sklearn.model_selection.
   - A RandomForestClassifier model is initialized, trained on the training data using fit(), and evaluated on the testing data using accuracy_score().
   - The accuracy of the model is printed.

5. Prediction and Visualization:
   - The model is used to make predictions on the test dataset, and the predictions are stored in the 'predictions' variable.
   - The number of survivors and non-survivors in the predictions are counted, and a bar plot is created to visualize the results.

## Conclusion

This project demonstrates the process of predicting the survival of Titanic passengers using a RandomForestClassifier model. The dataset is preprocessed by dropping irrelevant features, converting categorical features to numerical, filling missing values, and normalizing numerical features. The model is trained and evaluated, and predictions are made on the test dataset. The results are visualized using bar plots.

Feel free to modify the code and adapt it to your specific needs. Happy coding!

Note: It's important to cite the source of the dataset used, if applicable, and provide appropriate credits in your README file.

Thank you!!!