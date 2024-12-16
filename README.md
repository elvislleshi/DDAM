README for Accident Analysis and Prediction Project
Project Overview
This project explores the US-Accidents Dataset, a comprehensive collection of traffic accident data across 49 states in the United States from February 2016 to March 2023. The dataset contains approximately 7.7 million records, with 46 attributes describing various aspects of accidents, including location, weather conditions, traffic features, and more.

The project utilizes PySpark, a scalable framework for big data analysis, to perform:

Data understanding and preprocessing: Cleaning, feature engineering, and transformation of the dataset.
Clustering: Grouping accidents with similar attributes using KMeans.
Classification: Predicting accident severity using decision trees and logistic regression.
Regression: Estimating traffic duration with linear regression.
Dataset Description
The dataset includes the following key features:

Accident Information: ID, Severity, Start/End Time, Location (Lat/Lng).
Weather Data: Temperature, Wind Speed, Precipitation, Visibility, Weather Condition.
Traffic Infrastructure: Presence of signals, junctions, and other nearby structures.
Derived Features: Duration, Day/Night classification, weekend indicator.
Data Source
The dataset was obtained from the US-Accidents Dataset Page.

Project Objectives
Explore and preprocess the dataset to handle missing values and engineer new features.
Apply machine learning models for clustering, classification, and regression to gain insights into traffic accidents.
Evaluate and compare the performance of models to identify the most effective methods.
Workflow
1. Exploratory Data Analysis
Visualization of accident distribution by severity, location, time, and weather conditions.
Handling missing values with strategies such as grouping by location and weather conditions.
Feature transformation to address skewed distributions (e.g., log-transformations for numerical variables).
2. Clustering
Applied KMeans clustering to group accidents based on numerical attributes like distance, visibility, and precipitation.
Used the elbow method to determine the optimal number of clusters.
Clusters identified specific trends, such as severe accidents linked to long traffic durations.
3. Classification
Objective: Predict accident severity using:
Decision Tree Classifier
Logistic Regression
Tasks:
Binary classification of severe accidents (Severity = 4) vs. others.
Multi-class classification of severity levels.
Best performance was achieved with Decision Trees for high recall and balanced data.
4. Regression
Target variable: Traffic Duration.
Applied Log-Linear Regression with derived features such as traffic distance, visibility, and weather conditions.
Achieved moderate model performance, with insights linking roundabouts and severity to longer traffic durations.
Results
Clustering: Revealed patterns in accident severity, precipitation, and traffic duration.
Classification: Decision Trees outperformed Logistic Regression, achieving better recall for predicting severe accidents.
Regression: Identified key features influencing traffic duration, including severity and proximity to roundabouts.
Technology Stack
PySpark for scalable data processing and machine learning.
Matplotlib/Seaborn for data visualization.
Python for data transformation and modeling.
