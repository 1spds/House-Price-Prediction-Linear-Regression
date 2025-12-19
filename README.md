
# House Price Predictor

A beginner-friendly machine learning project that uses Linear Regression to predict housing prices based on various features in the California Housing dataset.

## Version 1.0: Linear Regression

### Objective

To build and evaluate a Linear Regression model that predicts median house prices in California districts based on various socio-economic and geographic features.

### Introduction

In this project, we aim to **predict housing prices in California** using **Linear Regression**, a fundamental machine learning algorithm for regression problems. The dataset contains various housing-related features such as location (latitude and longitude), total rooms, population, median income, and the median house value (our target variable).

### Project Workflow

1. **About this File**  
   A brief overview of the dataset, which includes housing data for California from the 1990 U.S. Census.

2. **Exploratory Data Analysis (EDA)**  
   We explore the dataset to understand its structure, identify patterns, correlations, and gain insights into the features that may influence house prices.

3. **Preprocessing**  
   This step involves selecting features and the target variable, handling missing values, and splitting the data into training and testing sets.

4. **Model Building**  
   A Linear Regression model is trained using the training dataset to learn the relationships between features and house values.

5. **Model Evaluation**  
   We evaluate the model's performance using metrics like MAE, MSE, and RMSE. Additionally, we visualize the results through:
   - **Actual vs Predicted Plot** to assess model accuracy  
   - **Residual Plot** to detect bias or patterns in errors

6. **Deployment**  
   The trained model is saved and later reloaded to make predictions on new data, simulating how the model could be used in a real-world application.

7. **Conclusion**
   In this project, we built a linear regression model to predict median house values in California using features such as median income, location, and housing characteristics.

   **Model Evaluation Results:**
   - Mean Absolute Error (MAE): **$51,049**

   - Mean Squared Error (MSE): **4.86 × 10⁹**

   - Root Mean Squared Error (RMSE): **$69,692**

   **Interpretation:**
   - The MAE of $51,049 implies that, on average, our model’s predictions are off by about $51k.

   - The RMSE gives more weight to larger errors and is around $69k, which is reasonable considering California housing prices.

   - The error values suggest that while the model captures the general trend in house prices, there is still significant room for improvement.

   **Key Observations:**
   - Median income has a strong correlation with house value and significantly influenced predictions.

   - Features like total rooms, bedrooms, and housing age also contributed but with lower impact.

   - Some prediction errors may stem from high variance or skewness in housing values and possible outliers.

   **Possible Improvements:**
   - Try non-linear models (e.g., polynomial regression, decision trees, random forest, gradient boosting).

   - Use feature engineering (e.g., rooms per household).

## Version 2.0: Polynomial Regression

### Objective

To build and evaluate a Polynomial Regression model that predicts median house prices in California districts by capturing non-linear relationships between socio-economic and geographic features, thereby improving prediction accuracy over a simple linear model.

### Introduction

In this version of the project, we enhance the housing price prediction model by applying Polynomial Regression. This approach captures nonlinear relationships among features by introducing interaction and squared terms. Polynomial regression is a generalization of linear regression and allows the model to better fit the complex patterns present in the data.

### Project Workflow

1. **About this File** 
   Same dataset as before: housing data from the 1990 U.S. Census for California, including features like latitude, longitude, total rooms, population, and median income.

2. **Exploratory Data Analysis (EDA)**  
   Already performed in the linear regression model; insights from EDA inform the polynomial feature construction.

3. **Preprocessing** 
   This step involves selecting features and the target variable, handling missing values, and splitting the data into training and testing sets.

4. **Model Building**  
   - Choosing the Optimal Degree for Polynomial Regression: To avoid both **underfitting** and **overfitting**, we evaluate polynomial regression models of increasing degree (from 1 to 9) and measure their performance on both the training and test sets.
   - Fitting Polynomial Regression
   - Predictions

5. **Model Evaluation**  
   We evaluate the model's performance using metrics like MAE, MSE, and RMSE. Additionally, we visualize the results through:
   - **Actual vs Predicted Plot** to assess model accuracy  
   - **Residual Plot** to detect bias or patterns in errors

6. **Deployment**  
   The trained model is saved and later reloaded to make predictions on new data, simulating how the model could be used in a real-world application.
7. **Conclusion**
   In this project, we built a linear regression model to predict median house values in California using features such as median income, location, and housing characteristics.

   **Model Evaluation Results:**
   - Mean Absolute Error (MAE): **$46,575**

   - Mean Squared Error (MSE): **4.39 × 10⁹**

   - Root Mean Squared Error (RMSE): **$66,298**

   **Interpretation:**
   - The MAE of $46,575 implies that, on average, our model’s predictions are off by about $46k, which is less than that predicted by linear regression model($51k)

   - The RMSE gives more weight to larger errors and is around $66k, which is reasonable considering California housing prices.

   - The error values suggest that while the model captures the general trend in house prices, there is still significant room for improvement.

   **Possible Improvements:**
   - Use feature engineering (e.g., rooms per household).
