# Crop Yield Prediction

The **Crop Yield Prediction** project is a machine learning-based application designed to predict crop yield based on historical agricultural data. By analyzing soil fertility characteristics, environmental factors, and crop type, this project provides valuable insights to optimize agricultural productivity and gives output of the estimated crop yield based on the inputs recieved.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Machine Learning Models](#machine-learning-models)
- [Dataset](#dataset)

---

## Overview

Crop yield prediction is crucial for improving agricultural practices and ensuring food security. This project leverages historical agricultural data, machine learning algorithms, and Flask to provide accurate yield predictions based on soil fertility characteristics and environmental conditions. The models used in this project include **Random Forest**, **Support Vector Machines (SVM)**, and **Decision Trees**. The application is containerized using **Docker** for easy deployment.

---

## Features

1. **Multi-Model Approach**:
   - Employs **Random Forest**, **SVM**, and **Decision Trees** to predict crop yield for increased reliability.

2. **Correlation of Data**:
   - Combines **soil fertility data** (e.g., nutrients like Ca, Mg, K, etc.) and **environmental factors** (e.g., temperature, humidity, rainfall) to ensure accurate predictions.

3. **Preprocessed Data**:
   - All input values of soil fertility are normalized between `0` and `1` for consistency and improved model performance.

4. **Flask API**:
   - A Flask-based REST API is used to provide predictions for user inputs.

5. **Containerized Deployment**:
   - Fully containerized using **Docker** to ensure a portable and scalable deployment.

6. **Saved Models**:
   - Pre-trained machine learning models are stored in `.pkl` files for fast and efficient inference.

---

## Tech Stack

### **Backend**
- **Python (Flask)**: Provides the API interface for the prediction service.
- **Machine Learning Models**: Implemented using Scikit-learn.
- **XML and YAML**: Used for configuration and data management.
- **Docker**: For containerizing and deploying the application.

### **Machine Learning**
- **Random Forest**: Ensemble learning method for accurate predictions.
- **Support Vector Machines (SVM)**: For classification and regression tasks.
- **Decision Trees**: Simple, interpretable model for yield prediction.

---

## Machine Learning Models

The project uses three machine learning models to predict crop yield:

1. **Random Forest**:
   - Highly accurate ensemble model.
   - Handles non-linear relationships well.

2. **Support Vector Machines (SVM)**:
   - Effective in high-dimensional spaces.
   - Ensures robust classification and regression.

3. **Decision Trees**:
   - Simple, interpretable model for yield prediction.
   - Captures non-linear relationships in the data.

The final prediction is based on the best-performing model for the given input data.

---

## Dataset

The project utilizes two datasets:

1. **Soil Fertility Data**:
   - Includes the following features (normalized between 0 and 1):
     - **Ca**: Calcium
     - **Mg**: Magnesium
     - **K**: Potassium
     - **S**: Sulfur
     - **N**: Nitrogen
     - **Lime**: Lime content
     - **C**: Carbon
     - **P**: Phosphorus
     - **Moisture**: Soil moisture
     - **Yield**: Crop yield value (target variable).

2. **Environmental Data**:
   - Includes:
     - **Temperature**
     - **Humidity**
     - **pH**
     - **Rainfall**
     - **Crop Type**

The datasets are correlated row-wise to ensure consistent mapping between soil and environmental data.

---