Hollywood Movie Profitability Prediction

This project predicts movie profitability using the Hollywood Most Profitable Stories dataset. The objective was to build and compare regression models while demonstrating a complete machine learning workflow, including data exploration, preprocessing, model training, evaluation, and interpretation of results.

Project Overview
The dataset contains information about Hollywood movies, including audience scores, Rotten Tomatoes ratings, worldwide gross revenue, genre, and lead studio. These features were used to predict movie profitability.

Target Variable:
Profitability

Dataset Information
Dataset: Hollywood Most Profitable Stories

Number of observations: 67 (after preprocessing)

Features: Worldwide Gross, Audience Score, Rotten Tomatoes Score, Genre, Lead Studio

Target: Profitability

Project Workflow
Loaded and explored the dataset.
Checked for missing values and duplicate records.
Handled missing values where necessary.
Removed outliers from the target variable using the IQR method.
Removed the Film column because it is a unique identifier and does not provide meaningful predictive information.
Applied One-Hot Encoding to categorical variables.
Standardized numerical features using StandardScaler.
Split the dataset into training and testing sets.
Trained and compared:
Linear Regression,
Ridge Regression,
Lasso Regression,
Evaluated model performance using MAE, RMSE, and R².
Examined feature coefficients to identify the most influential predictors.

Libraries Used
Python,
Pandas,
NumPy,
Matplotlib,
Seaborn,
Scikit-learn,

Model Evaluation
The models were evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score

Among the three models, Lasso Regression produced the best overall performance, although the improvement over Linear Regression and Ridge Regression was minimal. The results indicate that the available features have limited predictive power for accurately estimating movie profitability.


Key Findings
Most predictor variables had weak correlations with profitability.
Worldwide Gross showed the strongest positive relationship with profitability, followed by Audience Score.
Removing the Film column improved model generalization because movie titles are identifiers rather than predictive features.
The dataset lacks several important variables, including production budget, marketing expenditure, release timing, and competition, which likely contributed to the low predictive performance.
Comparing Linear Regression, Ridge Regression, and Lasso Regression demonstrated that changing the regression algorithm alone could not overcome the limitations of the available data.

Skills Demonstrated
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
This project demonstrates an end-to-end regression workflow and highlights the importance of understanding both model performance and dataset limitations. While the regression models achieved limited predictive accuracy, the analysis showed that the available features were insufficient to explain movie profitability effectively. The project emphasizes that successful machine learning depends not only on selecting appropriate algorithms but also on the quality, relevance, and completeness of the data.
