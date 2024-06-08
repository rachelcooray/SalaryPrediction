# SalaryPrediction

This project aims to predict the salaries of software developers based on their country, education level, and years of experience using machine learning models.

## Overview

This project predicts the salaries of software developers based on various inputs such as their country, education level, and years of experience. It uses data from the Stack Overflow Developer Survey 2020 and implements machine learning models for prediction.

## Project Structure

app.py: Main file to run the Streamlit application.
predict_page.py: Contains code for the prediction page of the app.
explore_page.py: Contains code for the explore page of the app.
saved_steps.pkl: Pickle file containing the trained model and label encoders.
survey_results_public.csv: Dataset used for training the model.

## Model

The model used in this project is a Decision Tree Regressor, fine-tuned using GridSearchCV. It predicts salaries based on three inputs:

Country: The country of the software developer.
Education Level: The education level of the software developer.
Years of Experience: The number of years the developer has been coding professionally.

## Data Processing
The data is preprocessed as follows:

Countries and education levels are label encoded.
Experience is cleaned and converted to numerical values.
Outliers in salary data are removed to improve model performance.

## Model Training
The model is trained using the Decision Tree Regressor with hyperparameter tuning using GridSearchCV. The model and encoders are saved in a pickle file (saved_steps.pkl) for later use.