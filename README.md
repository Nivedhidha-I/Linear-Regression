# Simple Linear Regression Model Recreation and Comparative Analysis

## Project Summary

This project involves the recreation of a Simple Linear Regression (SLR) model from foundational mathematics, without relying on high-level libraries like scikit-learn for the core algorithm. The goal was to build a comprehensive machine learning class (LinearRegression) capable of fitting data, making predictions, and calculating various accuracy metrics. The custom model was then used to analyze a real-world dataset (Flight Delay Times) and critically evaluate the impact of preprocessing techniques (Normalization/Standardization) and model configuration (Y-intercept inclusion) on predictive performance.

## Analytical & Pedagogical Focus 

This project demonstrates a deep, fundamental understanding of linear algebra and statistical methods underpinning supervised machine learning:

* Proves the ability to translate mathematical formulas (e.g., Ordinary Least Squares for calculating slope $M$ and intercept $C$) directly into functional Python code.

* Implemented and compared key model accuracy metrics to rigorously assess model fit.

* Investigated the practical effect of common data preprocessing steps on model stability and predictive power for a skewed dataset.

## Technical Scope & Components 

The project utilizes Python for all mathematical computation, modeling, and visualization:

* Language: Python

* Dataset Analyzed: Flight Delay Data

## Key Findings from Comparative Analysis

The analysis revealed that for the given right-skewed dataset:

* Applying Min-Max Normalization or Z-Score Standardization significantly decreased the R-squared score and predictive accuracy compared to using the raw, unscaled data.

* The model performed marginally better when the Y-intercept was explicitly set to zero (no_intercept = True), suggesting a very strong proportional relationship between departure and arrival delays.

* The default model, with no scaling and intercept exclusion, yielded the highest R-squared value of $\approx 0.928$ (and a high $r2\\_score$ on test data of $\approx 0.937$).
