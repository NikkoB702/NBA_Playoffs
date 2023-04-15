# NBA_Playoffs


![Jim-Mora-Playoffs](https://user-images.githubusercontent.com/80132877/232113495-cb8f6cfd-ec6e-475c-b2ef-31b746918460.jpg)


## NBA Team Performance Prediction Model

## Data Source and Data Collection

The dataset used in this project was sourced from Basketball-Reference, a comprehensive online database that provides a wealth of basketball statistics, scores, and historical records for both individual players and teams.

To collect the data, I employed web scraping techniques using the Pandas library in Python. Specifically, I utilized Pandas' read_html function to extract tabular data from the web pages of Basketball-Reference. The collected data consists of various team-level features and statistics, such as shooting percentages, turnovers, attendance, and overall team performance, for the NBA season under study.

It's important to note that the data scraping process was conducted in compliance with the terms of service of Basketball-Reference, and the dataset was utilized solely for the purpose of training and evaluating the machine learning model in this project.

Once the data was scraped and collected, it was cleaned, preprocessed, and organized into a structured format suitable for model training and analysis. The resulting dataset provided a solid foundation for developing the linear regression model that predicts the number of wins for NBA teams based on their statistics.

Use the advanced_stats dataset to achieve desired results!

This repository contains a machine learning model that predicts the number of wins ('W') for NBA teams based on their statistics. The dataset used for training and testing the model consists of various team-level features, such as shooting percentages, turnovers, and attendance.

##### Model Performance

The linear regression model was developed to predict the number of wins ('W') for NBA teams based on various team statistics, such as shooting percentages, turnovers, and attendance. The performance of the model was evaluated using a test dataset and multiple performance metrics to provide a comprehensive assessment of its predictive accuracy.

* Mean Squared Error (MSE): MSE measures the average squared difference between the predicted and actual values for the target variable ('W'). A lower MSE value indicates higher predictive accuracy. The model achieved an MSE of 3.575048502907954e-08 on the test dataset, which suggests that the model's predictions are very close to the actual values.

* KFold Cross-Validation RMSE Scores: To validate the model's performance and assess its generalization capability, KFold cross-validation was applied with five folds. The Root Mean Squared Error (RMSE) scores for each fold were [5.560466384069211e-08, 7.129072771899516e-14, 2.362665894334605e-13, 5.757881060779946e-14, 8.185131578576492e-13]. The mean RMSE score across all folds was 1.1121169497995546e-08. These low RMSE scores demonstrate the model's consistency across different data subsets.

* Mean Absolute Error (MAE): MAE measures the average absolute difference between the predicted and actual values. The model achieved a Mean MAE Score of 9.483454664946508e-09, which indicates that the model's predictions deviate minimally from the actual values.

* R-squared: R-squared measures the proportion of the variance in the dependent variable that is predictable from the independent variables. R-squared scores closer to 1 indicate better predictive performance. The model achieved an average R-squared score of 1.0 across all cross-validation folds, which suggests that the model can explain all of the variance in the target variable with the given features.

Overall, the model demonstrated impressive predictive accuracy across all performance metrics. The KFold cross-validation results validate the model's robustness and its ability to generalize well to new, unseen data.

##### Repository Structure

* data/: Contains the dataset used for training and testing the model.
* notebooks/: Contains Jupyter notebooks used for data exploration, preprocessing, and model training.
* scripts/: Contains Python scripts for data preprocessing, model training, and evaluation.
README.md: This file, providing an overview of the project and its results.

##### Getting Started

* Clone the repository to your local machine.
* Install the required Python packages using the provided requirements.txt file.
* Run the scripts in the scripts/ folder to preprocess the data, train the model, and evaluate its performance.

##### Dependencies

* Python 3.8 or later
* pandas
* numpy
* scikit-learn

##### Contributing
Feel free to submit issues or pull requests if you have any improvements or suggestions for the project.

##### License
This project is licensed under the MIT License. See the LICENSE file for more information.

The quality and integrity of the data and model were ensured through data exploration, handling missing values, and KFold cross-validation. The model achieved impressive results, making it a reliable tool for predicting NBA team performance based on team statistics.
