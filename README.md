Hollywood Movie Profitability Prediction
This project predicts movie profitability using the Hollywood Most Profitable Stories dataset. The objective was to build and compare regression models while demonstrating a complete machine learning workflow, including data exploration, preprocessing, feature engineering, model evaluation, and interpretation of results. 


Project Overview
The dataset contains information about Hollywood movies, including audience ratings, critic ratings, worldwide gross revenue, genre, and lead studio. These features were used to predict movie profitability.

Target variable:
Profitability

Dataset Information
Dataset: Hollywood Most Profitable Stories

Number of observations: 67 (after data cleaning)

Target: Profitability

Features Used
Worldwide Gross
Audience Score
Rotten Tomatoes Score
Genre
Lead Studio


Project Workflow
Loaded and explored the dataset.
Checked for missing values and duplicate records.
Filled missing values where necessary.
Removed outliers from the target variable (Profitability) using the IQR method.
Dropped the Film column because it is a unique identifier and does not generalize well for prediction.
Applied One-Hot Encoding to categorical variables (Genre and Lead Studio).
Standardized numerical features using StandardScaler.
Split the dataset into training and testing sets.
Trained and evaluated:
Linear Regression
Ridge Regression
Lasso Regression
Compared the models using MAE, RMSE, and R².
Examined feature coefficients to understand feature influence.


Libraries Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn


Model Evaluation
The models were evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score
Among the three models, Lasso Regression achieved the best performance, although the improvement over Linear Regression and Ridge Regression was small. Overall, the models showed limited predictive performance, indicating that the available features were insufficient to accurately predict movie profitability.


Key Findings
Correlation analysis showed that most features had weak relationships with Profitability.
Worldwide Gross exhibited the strongest positive correlation with profitability, followed by Audience Score.
The Film column was removed because it acts as a unique identifier rather than a meaningful predictive feature.
The limited predictive performance suggests that important variables such as production budget, marketing expenditure, release timing, and competition were not available in the dataset.
The project highlights the importance of feature quality and domain knowledge when building predictive machine learning models.


Skills Demonstrated:
Exploratory Data Analysis (EDA)
Data Cleaning
Missing Value Treatment
Outlier Detection and Removal (IQR)
One-Hot Encoding
Feature Scaling
Linear Regression
Ridge Regression
Lasso Regression
Model Evaluation (MAE, RMSE, R²)
Feature Importance Analysis
Machine Learning with Scikit-learn


Conclusion
This project demonstrates an end-to-end regression workflow and emphasizes the importance of interpreting model performance critically. Although the models achieved limited predictive accuracy, the analysis showed that the dataset lacked several key variables required to explain movie profitability. Comparing Linear Regression, Ridge Regression, and Lasso Regression illustrated how different regularization techniques behave when the underlying data provides limited predictive information.
