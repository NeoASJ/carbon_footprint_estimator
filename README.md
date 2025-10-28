# 🌍 Product Emission Prediction Using Machine Learning

## 🚀 Project Overview
The project combined data from the UK Greenhouse Gas Conversion Factors (2025) 🇬🇧 and a Kaggle e-commerce dataset 🛒 to create a synthetic dataset with product details and estimated carbon emissions. Data preprocessing in Python 🐍 involved cleaning, handling missing values, and creating new features like mass ⚖️ and emission factor 🌫️.

This project aims to predict the emissions of various products using machine learning regression models based on their mass and emission factor features. The target variable includes small product-specific noise 🔊 added to simulate measurement uncertainties or real-world variance.

## 📊 Data Description
- The dataset contains product-related features starting with prefixes `mass_` and `ef_`, representing weights ⚖️ and emission factors 🌫️, respectively.
- The target variable `Total Emissions` is perturbed with controlled noise based on the product category for realism 🔄.
- Products vary from electronics like "Air Conditioner" ❄️ and "Laptop" 💻 to apparel like "Shirt" 👕 and "Sneakers" 👟.

## 🤖 Models Used
- Random Forest Regressor 🌲
- LightGBM Regressor 💡
- CatBoost Regressor 🐱
- XGBoost Regressor ⚡

Each model is trained using limited hyperparameters to observe model behavior and comparative performance. The metric used for evaluation is the coefficient of determination \(R^2\) 📈.

## 🎯 Noise Addition Approach
Noise is added as a fraction (10%) of product-specific emission ranges randomly either positively or negatively to the target. This models real world data variability 🌍.

## ⚙️ Installation
Install dependencies using pip:


## ▶️ How to Run
- Load the dataset `processed.csv` into the script.
- Run the script to train the models and generate a bar plot comparing the \(R^2\) scores 📊.
- LightGBM model can be saved for future use 💾.

## 📈 Results and Visualization
The script plots the \(R^2\) scores of all models for quick comparison and insights.

## 🚀 Future Work
- Hyperparameter tuning to optimize each model 🎛️.
- Incorporation of additional features or different noise scaling 🔧.
- Extending models to classification or time series if data permits ⏳.

## 📫 Contact
For questions or collaborations, please reach out via email: your.email@example.com ✉️
