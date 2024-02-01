# Exclusive Product Classification Project

## Introduction
In today's competitive market, understanding what makes a product exclusive can provide valuable insights for businesses. This project aims to develop a classification model to categorize products as exclusive or non-exclusive based on various attributes. By leveraging machine learning techniques, we seek to identify patterns and factors contributing to a product's exclusivity.

[Documentation Details](https://github.com/Theofilusarifin/Exclusive-Product-Classification/blob/main/Documentation.pdf)

## Dataset Overview
- The dataset contains 8000 entries and 9 columns.
- Features include id, brand, category, rating, number of reviews, love, price, value price, and exclusive.
- Some columns have missing values, with the 'rating' column having the most missing data (95 entries).

## Data Preprocessing
- Missing values were observed in multiple columns and were addressed using either interpolation or dropping rows.
- Outliers were identified, especially in columns like 'rating', 'number_of_reviews', 'price', and 'value_price'.
- Categorical features like 'brand' and 'category' were analyzed for uniqueness and distribution.

## Exploratory Data Analysis
- Identified outliers and skewed distributions in numerical features.
- Observed correlations between features, noting high correlation between 'number_of_reviews' and 'love', and between 'price' and 'value_price'.
- Investigated the imbalance in the 'exclusive' label and proposed strategies for handling it.

## Feature Engineering
- Added additional features like 'mass_produced', 'kota_asal', 'bahan_baku', and 'limited_edition' to enhance predictive power.
- Decided to keep 'price' over 'value_price' due to higher correlation with the target variable.
- Selected 'love' over 'number_of_reviews' based on higher correlation with the target.

## Modeling
- Utilized machine learning algorithms like logistic regression, decision trees, and random forests for classification.
- Applied feature selection techniques to eliminate redundant or less relevant features.
- Evaluated model performance using appropriate metrics such as accuracy, precision, recall, and F1-score.

## Conclusion
This project provides insights into classifying products as exclusive or non-exclusive based on various features. Further improvements can be made by refining feature engineering, exploring advanced modeling techniques, and addressing class imbalance.
