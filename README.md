# Healthy-LifeStyle-Hackathon

<h2>Overview</h2>

This project aims to build and optimize a machine learning model to predict the health status (Healthy) of individuals based on various features such as age, BMI, smoking habits, and other lifestyle factors. The project involves data preprocessing, model training, evaluation, and hyperparameter tuning to achieve optimal performance.

<h2>Structure</h2>

The project consists of the following steps:

Data Import and Initial Exploration

Data Cleaning and Preprocessing

Feature Scaling

Data Splitting

Model Training and Evaluation

Hyperparameter Tuning

Final Model Evaluation

<h2>Data</h2>

Train_Data.csv: The training dataset containing the features and the target variable.

Test_Data.csv: The test dataset used for model evaluation.

<h2>Usage</h2>

**Data Import and Initial Exploration**

**Data Cleaning and Preprocessing**

Drop irrelevant columns (ID1, ID2, Any heriditary condition?) from both training and test datasets.

Extract and one-hot encode the categorical feature Food preference into multiple binary columns (DX1, DX2, DX3, DX4, DX5, DX6).

Encode categorical columns (Smoker?, Living in?) into numerical values.

Impute missing values in the training dataset using KNN imputer.

**Feature Scaling**

Apply StandardScaler to scale numerical features (Age, BMI, Specific ailments) in both training and test datasets.

**Data Splitting**

Split the training data into training and validation sets using train_test_split with a test size of 10%.

<h2>Model Training and Evaluation</h2>

Train multiple machine learning models (LogisticRegression, KNeighborsClassifier, etc.) on the training set.

Evaluate models using F1 score and accuracy metrics on the validation set.

Store model performance metrics in a DataFrame and sort by F1 score to compare model performance.

**Hyperparameter Tuning**

Perform hyperparameter tuning on the best-performing model, CatBoostClassifier, using RandomizedSearchCV to find the optimal set of hyperparameters.

Evaluate the tuned CatBoostClassifier on the validation set to obtain the best F1 score and accuracy.

<h2>Results</h2>

Best Model: CatBoostClassifier
Best Hyperparameters:
learning_rate: 0.05
l2_leaf_reg: 3
iterations: 300
depth: 6
border_count: 100
bagging_temperature: 0

<h2>Performance Metrics:</h2>

**F1 Score: 0.8829593693147362
Accuracy: 0.8510802469135802** 
