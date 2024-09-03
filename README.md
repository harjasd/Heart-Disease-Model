# Heart Attack Prediction Analysis

This repository contains the analysis and modeling work related to predicting heart attacks using a dataset sourced from Kaggle. The project focuses on identifying key predictors, performing exploratory data analysis (EDA), and building predictive models to aid in early detection and prevention of heart attacks.

## Dataset

The dataset includes 14 variables, both categorical and continuous, that relate to heart health indicators. The data spans multiple patient records and provides a comprehensive view of various factors that could contribute to heart attacks.

## Data Cleaning and Preparation

Before conducting the analysis, the dataset was thoroughly cleaned:
- Checked for and handled missing values and duplicate entries.
- Organized variables into categorical and continuous subsets.
- Focused on relevant columns, removing any unnecessary data.

This preparation ensured that the data was ready for accurate EDA and model building.

## Exploratory Data Analysis (EDA)

EDA was performed to gain insights into the relationships between different variables:
- **Histograms** were used to visualize the distribution of variables like cholesterol levels and maximum heart rate.
- **Box plots** and **scatter plots** helped identify potential associations between variables, such as chest pain type and heart attack likelihood.
- **Correlation analysis** was conducted to determine the strength of relationships between predictors and the output variable.

## Model Building

Two main models were developed:

1. **Logistic Regression Model**
   - Key predictors identified: chest pain type (cp), maximum heart rate (thalachh), and exercise-induced angina (exng).
   - The model demonstrated good discriminatory power with a high AUC score.

2. **Poisson Regression Model**
   - Focused on predicting the count of heart attacks.
   - Showed similar significant predictors but with a higher AIC score, indicating a relatively lower fit compared to the logistic regression model.

## Model Evaluation

The models were evaluated using several metrics:
- **AIC (Akaike Information Criterion)**: Used to compare the relative quality of the models.
- **McFadden's R-squared**: Provided insight into the model's goodness-of-fit.
- **Durbin-Watson test**: Checked for autocorrelation in the residuals, revealing some model limitations.

## Conclusion and Future Work

The analysis confirmed the importance of certain variables, such as chest pain type and maximum heart rate, in predicting heart attack events. However, issues like autocorrelation and potential overfitting suggest the need for further refinement.

### Future Improvements:
- Explore advanced techniques like **Gradient Boosting** to improve predictive accuracy.
- Address limitations such as autocorrelation and potential missing explanatory variables.
- Further normalization and detailed exploration of outliers to enhance model robustness.

## Repository Contents

- **Data Cleaning**: Scripts and code for initial data preparation.
- **EDA**: Visualizations and analysis scripts.
- **Modeling**: Code for Logistic Regression, Poisson Regression, and evaluation metrics.
- **Reports**: Detailed findings and analysis summaries.




