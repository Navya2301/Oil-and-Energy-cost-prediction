# Oil-and-Energy-cost-prediction
## Project Overview
This project aims to predict oil production rates using machine learning algorithms. The dataset used is from Volve P-12, consisting of various parameters that influence oil production. The goal is to create a model that accurately forecasts future oil rates, which can be used for economic analysis and investment planning

### Steps and Methodology
1. Data Import and Exploration: Imported the dataset and explored the data to understand the features and target variable.
Visualized how different factors vary with respect to the target variable, BORE_OIL_VOL.
2. Correlation Analysis: Calculated the correlation between the target variable and other features to identify the most influential factors.
3. Feature Selection: Selected features with a correlation coefficient between 0.2 and 0.9 to avoid leakage and multicollinearity.
4. Data Splitting: Split the data into training (first 3000 entries) and testing sets (remaining 291 entries) without shuffling to preserve the time series nature.
5. Feature Scaling: Scaled the features using StandardScaler to ensure the machine learning model treats features equally.
6. Modeling with Linear Regression: Trained a linear regression model but found it performed poorly, often predicting negative oil rates.
7. Modeling with Random Forest: Trained a random forest regressor which performed better, capturing the underlying trends more accurately.
### Visualization and Analysis: 
Visualized the predictions against actual data for both training and testing sets to evaluate model performance. Discussed potential reasons for model performance and the importance of domain knowledge.
 ### Results
1. Linear Regression: The linear model failed to capture the complexity of the data, leading to inaccurate predictions.
2. Random Forest: The random forest model provided a more reliable forecast, suggesting better generalization and understanding of the data patterns.
### Economic Implications
The project demonstrates how machine learning models can be used to predict future oil rates. By integrating these predictions with current oil prices, stakeholders can forecast future cash flows and make informed economic decisions.
### Future Work
Explore more complex models and feature engineering techniques to improve prediction accuracy.
Incorporate domain knowledge to better understand and model the relationships between features and the target variable.
### Getting Started
1. Clone the repository.
2. Install the required packages using pip install -r requirements.txt.
3. Run the Oil_rates_prediction.ipynb notebook to reproduce the analysis and predictions.
