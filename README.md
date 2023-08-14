# Comparing_ML_Models
# Titanic Survival Prediction using Machine Learning
### Titanic

This repository contains a machine learning project that focuses on predicting the survival outcomes of passengers aboard the Titanic. The project utilizes the famous Titanic dataset from Kaggle, which has been a popular dataset for introductory machine learning and data analysis tasks.

## Table of Contents
- [Introduction](#introduction)
- [Data Source](#data-source)
- [Data Preprocessing](#data-preprocessing)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction
The sinking of the Titanic is one of the most infamous shipwrecks in history. This project aims to build predictive models that can determine the likelihood of survival for passengers based on various features such as age, gender, class, etc. The project employs a variety of machine learning models and techniques to achieve this goal.

## Data Source
The dataset used in this project is the Titanic dataset, which can be found on Kaggle: Titanic: Machine Learning from Disaster. The dataset contains information about passengers, including whether they survived or not, as well as features such as age, gender, class, and more.

## Data Preprocessing
Before feeding the data into machine learning models, several preprocessing steps were performed:

- **Handling missing values**: The Age and Embarked columns had missing values, which were imputed using appropriate strategies.
- **Feature scaling**: The continuous feature Age was discretized to create age groups, simplifying its representation.
- **Categorical encoding**: Categorical variables like Sex and Embarked were encoded into numerical values.

## Feature Engineering
- To enhance the predictive power of the models, new features were created, such as family size and whether a passenger was traveling alone. These engineered features provide additional information for the models to learn from.

## Modeling
A variety of machine learning models were applied to the preprocessed data, using the scikit-learn library. The list of models used includes:

- **Ensemble Methods** : AdaBoostClassifier, BaggingClassifier, ExtraTreesClassifier, GradientBoostingClassifier, RandomForestClassifier
- **Gaussian Processes**: GaussianProcessClassifier
- **GLM (Generalized Linear Models)**: LogisticRegressionCV, PassiveAggressiveClassifier, RidgeClassifierCV, SGDClassifier, Perceptron
- **Naive Bayes**: BernoulliNB, GaussianNB
- **Nearest Neighbors**: KNeighborsClassifier
- **SVM (Support Vector Machines)**: SVC, NuSVC, LinearSVC
- **Decision Trees**: DecisionTreeClassifier

## Results
After training and evaluating the models, it was discovered that the top three performing models in terms of accuracy were:

1. Bagging Classifier
2. Linear SVC (Support Vector Classifier)
3. Logistic RegressionCV

## Conclusion
The Titanic survival prediction project demonstrates the application of various machine learning models on real-world data. The results highlight the potential of ensemble methods, linear SVC, and logistic regression in predicting survival outcomes. This project serves as an excellent starting point for individuals interested in understanding data preprocessing, feature engineering, and model evaluation within the context of a classic dataset.
