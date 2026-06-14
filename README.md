# Airfoil Noise Prediction ML Pipeline

## Project Overview

This project demonstrates an end-to-end Machine Learning pipeline built using Apache Spark for predicting airfoil noise levels. The dataset used is a modified version of the NASA Airfoil Self-Noise dataset, which contains aerodynamic and acoustic measurements collected from airfoil experiments.

As a Data Engineering project, the focus is on data preparation, ETL processing, machine learning pipeline creation, model training, evaluation, and model persistence.

## Objectives

- Load and analyze the airfoil noise dataset.
- Perform data cleaning and preprocessing.
- Remove duplicate records.
- Handle missing or null values.
- Create feature vectors using Spark ML transformers.
- Build a Machine Learning pipeline.
- Train a regression model to predict sound levels.
- Evaluate model performance using regression metrics.
- Save the trained model for future inference and deployment.

## Technologies Used

- Python
- Apache Spark (PySpark)
- Spark MLlib
- Machine Learning Pipelines
- DataFrame API

## Workflow

### 1. Data Ingestion

The airfoil dataset is loaded into a Spark DataFrame for distributed processing.

### 2. Data Cleaning

The dataset is cleaned by:

- Removing duplicate records.
- Removing rows containing null values.
- Validating data quality before model training.

### 3. Feature Engineering

Relevant input features are assembled into a single feature vector using Spark ML transformers.

### 4. Model Training

A regression model is trained to predict the target variable:

**SoundLevel**

based on the following input features:

- Frequency
- Angle of Attack
- Chord Length
- Free Stream Velocity
- Suction Side Displacement Thickness

### 5. Model Evaluation

The trained model is evaluated using regression performance metrics to measure prediction accuracy.

### 6. Model Persistence

The final trained model is saved and can be reloaded later for inference or deployment.

## Expected Outcome

The resulting machine learning pipeline can accurately predict airfoil sound levels based on aerodynamic characteristics, providing a scalable solution for engineering analysis and noise prediction.
