# ml-forecasting-veggies
Forecasting vegetable prices using economic indicators and time series models (VAR, VECM, ARDL).

# Vegetable Price Forecasting Using Macroeconomic Indicators

## Overview
This project is aimed at forecasting vegetable prices using key economic indicators, including the Exchange Rate, Headline Inflation, and Fuel Price (Diesel). The objective is to predict future vegetable price trends by capturing the relationships between these macroeconomic variables and the price fluctuations of vegetables. This forecasting process employs several advanced time series modeling techniques, including Vector Autoregression (VAR), Vector Error Correction Model (VECM), and Autoregressive Distributed Lag (ARDL), to model both short-term and long-term dependencies in the data.

## Key Components of the Project

### Time Series Analysis:

1. **VAR (Vector Autoregression):**
   - Used for modeling the interdependencies among multiple time series variables without requiring any specific assumptions about the direction of the relationships.
   
2. **VECM (Vector Error Correction Model):**
   - Applied when cointegration is found between the variables, allowing for both short-term adjustments and long-term equilibrium relationships between the variables.
   
3. **ARDL (Autoregressive Distributed Lag):**
   - Helps model the relationship between current and past values of the dependent variable and independent variables, allowing for more flexible lags and capturing both short-term and long-term dynamics.

### Principal Component Analysis (PCA):

- **Dimensionality Reduction:**  
  The project integrates Principal Component Analysis (PCA) to reduce the complexity of the multivariate economic data. PCA identifies the most significant components that explain the majority of the variation in the dataset, effectively simplifying the feature space while retaining important information. This step is critical for improving the stability and accuracy of predictive models by eliminating noise and reducing multicollinearity in the dataset.
  
- **Feature Extraction:**  
  PCA transforms the original features (such as Exchange Rate, Inflation, etc.) into principal components, which are then used in the forecasting models. These components represent the underlying patterns that drive the changes in vegetable prices, which aids in more accurate and efficient modeling.

## Evaluation Metrics:
The performance of the models is evaluated using common regression metrics such as **Root Mean Squared Error (RMSE)** and **R-squared (R²)**. These metrics provide insights into the prediction accuracy and goodness of fit, allowing for comparison between different models and forecasting strategies.

## Forecasting:
Once the models are trained, the system predicts future values of economic indicators (like the Economic Index) and vegetable prices. The forecasts are visualized to help analysts and decision-makers understand expected price movements and make informed decisions about market strategies, pricing, and policy planning.

## End-User Application:
The results from this analysis can be useful for **market analysts, policymakers, and farmers**, providing them with data-driven insights into how changes in macroeconomic indicators influence vegetable prices. This knowledge is critical for anticipating market trends and making informed decisions about pricing strategies and market interventions.

## Techniques and Methods:

- **Cointegration Testing:**  
  Johansen Cointegration tests are applied to determine whether long-term equilibrium relationships exist between the economic indicators and vegetable prices. If cointegration is found, VECM is employed to capture the adjustment dynamics.
  
- **Forecasting with PCA Components:**  
  PCA is leveraged to reduce the dimensionality of the dataset, thereby enhancing the efficiency of the ARDL, VAR, and VECM models and improving forecasting accuracy.

## Objective:
The main goal is to develop a robust system for forecasting vegetable prices based on macroeconomic indicators while ensuring that the complexities of the data are effectively handled. By combining time series models with PCA, the project aims to provide more accurate, interpretable, and efficient price forecasts, which are vital for stakeholders in the agricultural and economic sectors.

