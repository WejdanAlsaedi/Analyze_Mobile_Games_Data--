# Analyze_Mobile_Games_Data--
## Abstract
The purpose of this project is to do exploratory data analysis (EDA) and using machine learning models to help games developers when they create and develop games to predict their rating before published it. I worked with App Store Games dataset provide by Kaggle open dataset, using three regression models to achieve results for this problem. Finally, comparing the results of the models and choosing the best model got good results.
## Design
This project originates from the App Store Games dataset. The data is provided by Kaggle open dataset, and presents an information of games in apple app store. Predicting user rating via machine learning models would enable game developers to predict the user rating of their games before they are published or predict their user rating after they are developed.
## Data
The dataset contains about 187k unique games with 23 features for each. These are features will be used 'name_app', 'developer', 'age_rating', 'size', 'price', 'purchases', 'languages', 'sub_category', 'version_count', 'rating_avg', 'rating_count'.
## Algorithms
1-Clean the dataset 

Includes removing duplicate or unnecessary data, fixing inconsistencies and typos and dealing missing data

2- Exploratory Data Analysis (EDA) 

3- Models

Using three regression models LinearRegression, DecisionTreeRegressor and RandomForestRegressor
with StandardScaler to make sure to scale features before fitting them.

3- Model Evaluation and Selection

The split to 80% for training and 20% for testing and using K-Folds cross-validator with 5-fold cross validation just on the training portion only.
The best model after cross_val_score is to Random forest regressor with r^2: 0.78

Final resulte for predict testset on random forest regressor with estimator equal 150 are:
r^2: 0.79
Mean squared error: 0.90

## Tools
* Numpy and Pandas for data manipulation
* Scikit-learn for modeling
* Matplotlib and Seaborn for plotting
