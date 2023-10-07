# 🌊 Sea Level Prediction Model 🌊

## 🚀 Introduction

Welcome to the Sea Level Predictor Project! 🌊📈 Climate change has been a spotlight issue, bringing forth various environmental challenges that impact ecosystems, human communities, and economies. One such notable impact is the rise in global sea levels, which poses significant threats to coastal regions around the world. Understanding and predicting sea levels is paramount to developing mitigation strategies and ensuring the sustainability of impacted regions.

This project leaps into the profound depths of machine learning and data analytics to unravel patterns and develop predictive models concerning sea levels. Utilizing a dataset enriched with chronological sea level measurements and potentially influencing variables, we embark on a journey through systematic data exploration, feature engineering, model development, and deployment, all while adhering to the comprehensive CRISP-DM methodology.

Deep Dive: Explore a detailed journey through my project in my Medium article: 

[Rising Tides, Sinking Cities: A Data-Driven Dive into Predicting Sea Levels](https://medium.com/@sidsanc4998/rising-tides-sinking-cities-a-data-driven-dive-into-predicting-sea-levels-b50803dfca59)

[Chat Script](https://chat.openai.com/share/8e258e77-5313-4058-a99b-37b52f6353c8)

## 🧐 Problem Statement

The consistent rise in global sea levels has been attributed to various factors such as global warming, glacier melting, and other environmental phenomena. The ability to predict sea levels is crucial in formulating and implementing preventive and adaptive measures, particularly in regions that are severely affected by rising waters.

## 🎯 Objective: 
The primary objective of this project is to develop a predictive model that can accurately forecast sea levels based on historical data and influential variables.

## 🔍 Challenges:

Developing a model that accurately captures the underlying patterns and complexities of the influencing variables.
Ensuring the model is robust and generalizable to various temporal and spatial scenarios.
Implementing a user-friendly interface that effectively communicates the model’s predictions to end-users, facilitating data-driven decision-making.

### Table of Contents

- [Overview](#overview)
- [Data Exploration & Analysis](#data-exploration--analysis)
- [Feature Engineering & Model Tuning](#feature-engineering--model-tuning)
- [Model Deployment & UI](#model-deployment--ui)
- [Getting Started](#getting-started)
- [Contributing & Feedback](#contributing--feedback)
- [License](#license)


## Overview

This project involves predicting sea levels using a dataset from Kaggle. The CRISP-DM methodology was used to guide the process, ensuring a structured and comprehensive approach to the data science tasks.

##  Data Exploration & Analysis

### Data Loading

The data was loaded from a CSV file named sealevel.csv.
This dataset contains various variables related to sea level measurements over time.

Dataset Variables

Time: The timestamp associated with each measurement.

GMSL (GIA applied): Global Mean Sea Level (GMSL) with the Glacial Isostatic Adjustment (GIA) applied.

GMSL (NO GIA applied): GMSL without the GIA applied.

### Data Cleaning & Preprocessing

Handled missing values.

Detected and addressed outliers using the IQR method.

Conducted time-based train-test splitting to ensure the model is validated in a realistic manner.

### Data Visualization
Plotted time series trends of the sea level.

Visualized the distribution and relationships of key variables.

Decomposed the time series to observe underlying trends and seasonality.

##  Feature Engineering & Model Tuning

### Feature Engineering

Introduced lag variables and rolling mean features to capture temporal patterns.

Implemented polynomial features for capturing non-linear relationships.

Explored other rolling features like rolling standard deviation.

### Model Tuning

Used a Random Forest Regressor for modeling.

Evaluated the model's performance against a baseline to ensure predictive capability.

Fine-tuned the model using Randomized Search for hyperparameter optimization.

##  Model Deployment & UI
### Model Deployment
The trained model can be deployed as a RESTful API using Flask.

Docker can be used for containerizing the app, ensuring consistent behavior across environments.

Cloud platforms like AWS or Heroku can host the app for scalability and on-demand access.

### User Interface
A simple web UI was proposed using Flask and HTML/CSS.

Users can input data features through a form and receive sea level predictions.

###  Model Evaluation
- MAE: 6.85

- MSE: 75.58

- R²: -0.56

## Getting Started
To get a local copy up and running, follow these steps:

Clone the repository.

Install the required packages.

Run the Flask app.

Navigate to http://127.0.0.1:5000/ on your browser.

## Contributing & Feedback
Contributions, issues, and feature requests are welcome!

For major changes, please open an issue first to discuss what you would like to change. Feedback on the model, features, and potential improvements is highly appreciated.


## 🙏 Acknowledgements
Credits for code inspirations, dataset providers, and any other support.
