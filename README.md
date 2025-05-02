# Body Performance Classification

A data science project analyzing and classifying body performance into four classes based on physical and physiological attributes.

## Project Overview

This project applies machine learning techniques to classify individuals' physical performance based on various measurements including body composition, cardiovascular health, and strength indicators. The performance is categorized into four classes (A, B, C, D) where A represents the highest performance level and D the lowest.

## Dataset

The dataset contains 13,393 records with the following features:
- Age
- Gender (M/F)
- Height (cm)
- Weight (kg)
- Body fat percentage
- Blood pressure (diastolic, systolic)
- Performance measurements:
  - Grip force
  - Sit and bend forward (cm)
  - Sit-ups count
  - Broad jump (cm)

## Methodology

The analysis follows these steps:
1. **Data Preprocessing**
   - Handling duplicates
   - Outlier detection and treatment
   - Exploratory data analysis

2. **Statistical Analysis**
   - Distribution analysis
   - Correlation analysis
   - ANOVA tests to compare attributes across performance classes
   - Gender-based performance comparison

3. **Model Development**
   - Data balancing using SMOTE
   - Training multiple classification models:
     - Multinomial Logistic Regression
     - Random Forest
     - XGBoost
   - Model evaluation and comparison

## Key Findings

- Significant differences in physical attributes exist across performance classes
- Gender has a strong influence on physical performance metrics
- High performers (Class A) show superior strength indicators, endurance, and body composition
- Tree-based models outperform logistic regression for this classification task

## Technologies Used

- R programming language
- Libraries:
  - tidyverse (data manipulation)
  - caret (machine learning)
  - randomForest, xgboost (modeling)
  - themis (data balancing)
  - corrplot, ggplot2 (visualization)

## Files

- `bodyPerformance.Rmd`: R Markdown file containing all code and analysis
- `bodyPerformance.pdf`: Rendered report with visualizations and findings
- `bodyPerformance.csv`: Raw dataset
- `Report.pdf`: Comprehensive project report

## How to Run

1. Clone this repository
2. Open the R Markdown file in RStudio
3. Install required packages:
   ```R
   install.packages(c("tidyverse", "janitor", "corrplot", "gridExtra", "nnet", 
                     "caret", "rpart.plot", "randomForest", "xgboost", 
                     "themis", "tidymodels", "VIM", "lmPerm"))
   ```
4. Run the entire R Markdown file or individual chunks 
