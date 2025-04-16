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

