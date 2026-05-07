# 🏡 Real Estate Rent Prediction Pipeline

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-FF6F00?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

An end-to-end Data Science and Machine Learning project designed to extract, analyze, and predict real estate rental prices. This project demonstrates a complete machine learning lifecycle, starting from raw web-scraped data to building robust predictive models using both Regression and Classification techniques.

## 🚀 Project Overview

The real estate market is highly dynamic. This project aims to accurately predict rental prices by analyzing housing features (such as location, square footage, room count, etc.). The dataset is custom-built by scraping real-world listings from **Hepsiemlak** (a major Turkish real estate platform), ensuring the models are trained on current and practical market data.

## 🧠 End-to-End ML Pipeline (Key Features)

This repository is structured linearly to reflect a professional data science workflow:

1. **🕸️ Data Extraction (`data_extraction.ipynb`):**
   * Automated web scraping to collect raw housing listings directly from the Hepsiemlak platform.
   * Compiles the raw data into initial datasets (`hepsiemlak.csv`).

2. **🧹 Data Cleaning & Preprocessing:**
   * Handling missing values, parsing strings to numerical formats, and removing outliers.
   * Outputs refined datasets (`data_cleaned.csv` and `processed_data.csv`) ready for algorithmic ingestion.

3. **📊 Statistical Analysis & EDA (`statically_analyze.ipynb`):**
   * Exploratory Data Analysis (EDA) to discover underlying patterns, feature correlations, and data distributions.
   * Visualizing the impact of different housing features on rental prices.

4. **📈 Regression Modeling (`regression.ipynb`):**
   * Training supervised machine learning models to predict the *exact continuous value* of rent prices.
   * Model evaluation using metrics like RMSE, MAE, and R² Score.

5. **🗂️ Classification Modeling (`classification.ipynb`):**
   * Categorizing properties into specific rent price tiers/brackets (e.g., Affordable, Moderate, Expensive).
   * Evaluating classification performance using Accuracy, Precision, Recall, and F1-Scores.

## 📂 Repository Structure

```text
rentPredictionApplication/
│
├── Notebooks/
│   ├── data_extraction.ipynb      # Web scraping & data collection logic
│   ├── statically_analyze.ipynb   # Exploratory Data Analysis (EDA)
│   ├── regression.ipynb           # Continuous rent price prediction models
│   └── classification.ipynb       # Categorical price tier prediction models
│
├── Datasets/
│   ├── hepsiemlak.csv             # Raw scraped data (multiple versions)
│   ├── data_cleaned.csv           # Data after handling nulls and formatting
│   └── processed_data.csv         # Final encoded data ready for ML models
│
└── .idea/                         # IDE configuration files
