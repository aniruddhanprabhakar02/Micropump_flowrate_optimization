# Micropump Flowrate Optimization

This project focuses on identifying optimal pressure–time (`Pc`, `Ts`) configurations for micropump actuation using machine learning–based predictive analysis.

## Overview

The workflow extracts statistical flowrate features from experimental datasets and applies machine learning techniques to classify and rank optimal operating conditions for micropump performance.

## Features

- Automated feature extraction from flowrate experiments
- Unsupervised clustering for auto-label generation
- Hyperparameter optimization using Optuna
- Predictive classification using XGBoost
- Performance evaluation using:
  - AUC-ROC
  - Confusion Matrix
  - Precision-Recall Curve
- Ranking of optimal pressure-time combinations
- Visualization of model predictions and evaluation metrics

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Optuna
- Matplotlib
- Seaborn

## Dataset Availability

This repository contains a sample subset of the experimental dataset used for model development and evaluation.

The full dataset is not publicly released due to confidential research and proprietary experimental constraints. However, the provided sample data preserves the structure and preprocessing workflow required to understand and reproduce the implemented methodology.

## Workflow

1. Load and preprocess experimental micropump data
2. Extract statistical flowrate features:
   - Mean Flowrate
   - Standard Deviation
   - Flowrate Range
3. Generate labels using clustering techniques
4. Train and optimize the XGBoost classifier
5. Evaluate model performance
6. Rank pressure-time configurations based on predicted optimality

## Output

The model predicts and ranks the most efficient micropump actuation settings for improved flowrate performance and system optimization.

## Future Improvements

- Real-time actuator integration
- Deep learning-based optimization
- Adaptive control system implementation
- IoT-enabled monitoring and feedback control