# Dissertation-Coventry-University-2025
A hybrid machine learning pipeline for real estate price prediction, integrating structured data and CLIP-extracted visual features using Random Forest, XGBoost, and Gradient Boosting models.

# Real Estate Price Prediction using Hybrid Machine Learning Models

This repository contains the codebase for the undergraduate dissertation project titled:

**"An AI-Powered Framework for Predicting Real Estate Prices: Integrating Structured Data and Visual Features"**

## Project Overview

This project investigates a hybrid machine learning approach to property price prediction by combining structured real estate data with image-based visual features. The goal is to enhance prediction accuracy by leveraging both quantitative and qualitative characteristics of properties.

Structured data (e.g., square footage, location, number of bedrooms) is combined with visual features extracted from exterior property images using OpenCLIP, a vision-language model. Multiple tree-based regression algorithms are evaluated and compared.

## Methodology

- Data preprocessing and outlier handling on structured features
- Feature extraction from property images using OpenCLIP with prompt-based scoring
- Engineering contextual features (e.g., city average price)
- Merging structured and visual data into a unified dataset
- Model training using:
  - Random Forest
  - XGBoost
  - Gradient Boosting Regressor
- Stratified K-Fold Cross-Validation for model evaluation
- Hyperparameter tuning via Random Search and Grid Search

## Visual Features Extracted

- Garage presence score
- Greenery score
- Window count score
- Driveway or yard presence score

These were derived from exterior property images through OpenCLIP zero-shot classification.

## Project Structure

## Setup Instructions

1. Clone the repository: https://github.com/Talal-Abuabdu/Dissertation-Coventry-University-2025
2. Install dependencies: pip install -r requirements.txt 
3. Launch the Jupyter Notebook:


Alternatively, run the notebook in Google Colab (recommended for GPU access).

## Results Summary

The best performance was achieved using a Grid Search-tuned XGBoost model.

| Model               | Avg MAE ($) | R² Score | MAE as % of Mean Price |
|--------------------|-------------|----------|------------------------|
| Random Forest       | 63,949      | 0.835    | 10.26%                 |
| XGBoost (Tuned)     | 56,836      | 0.844    | 9.12%                  |
| Gradient Boosting   | 61,699      | 0.841    | 9.90%                  |

## License

This project is provided for academic reference purposes only. Redistribution or commercial use is not permitted without explicit permission.

## Citation

Abu Abdo, T. E. K. H. (2025). *Real estate price prediction with hybrid machine learning models* [Source code]. GitHub. https://github.com/Talal-Abuabdu/Dissertation-Coventry-University-2025

## Acknowledgements

- Supervisor: Dr. Worrallo  
- Visual Feature Extraction: OpenCLIP  
- Dataset Source: Kaggle – House Prices and Images (SoCal) available via the link below
- https://www.kaggle.com/datasets/ted8080/house-prices-and-images-socal




