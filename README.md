# Accurate Energy Demand Prediction for Smart Cities using Deep Learning

## Overview
This repository contains my MSc Dissertation project, which investigates the efficacy of various forecasting architectures in predicting urban energy consumption. The study compares 11 different models—ranging from statistical baselines to sophisticated Deep Learning LSTMs—across minute, hourly, and daily data frequencies.

**Key Achievement:** Conducted a comprehensive comparative analysis of accuracy vs. computational cost using a dataset of ~2 million records. 
**Grade:** Distinction.

---

## Project Structure
The project is divided into specialized notebooks to manage computational load and runtime requirements:

1. **`DataPreparation.ipynb`**: End-to-end pipeline for loading, cleaning, and feature engineering.
2. **`InvestigatingMissingValues.ipynb`**: Analysis of data missingness (MNAR, MCAR, MAR).
3. **`BaselineModels.ipynb`**: Implementation of Naive Forecast, SARIMA, Holt-Winters, MLR, and Random Forest.
4. **`IntermediateModels.ipynb`**: Implementation and tuning of MLP, SVM, and XGBoost.
5. **`AdvancedModels.ipynb`**: Deep Learning pipeline featuring Simple, Stacked, and Bidirectional LSTM networks.

---

## Dataset
* **Source:** [UCI Machine Learning Repository - Individual Household Electric Power Consumption](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)
* **Size:** ~2,049,280 observations.
* **Features:** Real-time electricity consumption, voltage, and sub-metering values.

---

## Models & Performance
I evaluated the following architectures:
* **Statistical/ML Baselines:** SARIMA, Holt-Winters, Random Forest (RFR).
* **Intermediate ML:** Support Vector Machine (SVM), XGBoost, Multi-Layer Perceptron (MLP).
* **Deep Learning:** Simple LSTM, Stacked LSTM, and Bidirectional LSTM.

> **Note on Computational Cost:** Advanced models were trained using a **T4 GPU** runtime. High-RAM environments were utilized for the Random Forest and XGBoost hyperparameter tuning phases.
