# Netflix Movies & TV Shows Classification

## Overview
This project analyzes the Netflix dataset and applies classification techniques.  
The main goals were:
- Data cleaning and preprocessing  
- Feature engineering (encoding categorical data)  
- Classification tasks:  
  - Predicting **Type** (Movie or TV Show)  
  - Predicting **Rating group** (Family, Teens, Adults)  

## Dataset
- Source: Netflix Movies and TV Shows (Kaggle)  
- Features used: `release_year`, `duration`, `rating`, `listed_in`  

## Steps
1. Data cleaning (handling missing values, simplifying ratings)  
2. OneHotEncoding for categorical features  
3. Applied classification models: Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, KNN  

## Results

### Type Classification (Movie vs TV Show)
| Model                | Train Acc | Test Acc |
|-----------------------|-----------|----------|
| Logistic Regression   | 99.37%    | 98.18%   |
| Decision Tree         | 100%      | 99.54%   |
| Random Forest         | 100%      | 99.60%   |
| Gradient Boosting     | 99.33%    | 99.09%   |
| KNN                   | 98.77%    | 98.29%   |

### Rating Group Classification (Family, Teens, Adults)
| Model                | Train Acc | Test Acc |
|-----------------------|-----------|----------|
| Logistic Regression   | 64.57%    | 61.93%   |
| Gradient Boosting     | 65.72%    | 61.64%   |
| KNN                   | 67.82%    | 53.52%   |

## Key Insights
- Movie vs TV Show classification achieved very high accuracy.  
- Rating group prediction was less accurate, suggesting more features (e.g., text analysis) could help.  

## Future Work
- Use NLP on the `description` column.  
- Try deep learning models.  
- Build a small web app for predictions.  
