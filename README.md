# FBI Time Series Forecasting
This project focuses on developing a machine learning model to predict crime rates based on historical patterns. The goal is to assist law enforcement agencies in efficiently allocating resources and potentially preventing unlawful situations.

## Problem Statement

In an effort to address rising crime rates, this project aims to build a crime prediction model using time series forecasting techniques. The model will leverage past crime data to identify trends and predict future occurrences, thereby aiding in proactive crime prevention and law enforcement strategies.

## Scope

This project can be expanded in the future to include predictions for various types of incidents, potentially including terrorist attacks, and could be a valuable tool for assisting in the security planning for foreign dignitaries.

## Project Process

The key steps followed in this project are:

1.  **Data Collection, Cleaning, and Preprocessing:** Gathering and preparing the raw crime data, handling missing values, and transforming features.
2.  **Exploratory Data Analysis (EDA):** Visualizing and analyzing the dataset to understand crime patterns, distributions, and relationships between variables.
3.  **Model Selection:** Choosing appropriate machine learning algorithms for time series forecasting.
4.  **Model Training:** Training the selected models on the preprocessed data.
5.  **Evaluation and Results:** Assessing the performance of the trained models using relevant evaluation metrics.
6.  **Implementation and Deployment (Future Work):** Discussing potential steps for deploying the trained model for real-world use.

## Data

The dataset used in this project includes information about various crime incidents, including:

*   **TYPE:** Category of the crime (e.g., "Other Theft").
*   **HUNDRED\_BLOCK:** Street block where the crime occurred.
*   **NEIGHBOURHOOD:** Neighborhood where the crime took place.
*   **X, Y, Latitude, Longitude:** Coordinates of the crime location.
*   **HOUR, MINUTE:** Time of the day when the crime occurred.
*   **Date:** Date when the crime happened.

## Data Analysis and Visualizations

The project includes extensive data analysis and visualization to gain insights into crime patterns. Some key visualizations include:

*   Crime type distribution
*   Frequency of crime by day, month, and year
*   Crime frequency by neighborhoods
*   Relationships between crime types and time (hour, month)
*   Crime distribution by location
*   Crime trends over time
*   Crime frequency with time (3D plot)
*   Crime vs. hour and month (heatmap)
*   Pairwise relationships between temporal variables

## Hypothesis Testing

Hypothesis testing was performed to validate assumptions about crime patterns, such as the relationship between weather conditions and crime rates.

## Feature Engineering and Data Preprocessing

The following data preprocessing steps were performed:

*   Handling Missing Values (Median imputation was used)
*   Handling Outliers (IQR method was used)
*   Categorical Encoding (One-Hot Encoding was used)
*   Feature Manipulation (Creating features like `NEIGHBOURHOOD_freq` and `Crime_Hotspot`)
*   Feature Selection
*   Data Transformation (Log transformation was applied to skewed numerical columns)
*   Data Scaling (Standardization was used)
*   Data Splitting (80% training, 20% testing)
*   Handling Imbalanced Dataset

## Machine Learning Models

Several machine learning models were implemented and evaluated for crime prediction:

*   **Random Forest Classifier:** Used for crime type prediction.
*   **Linear Regression:** Used for predicting crime frequency based on temporal features.
*   **Gradient Boosting Regressor (GBR):** Another regression model explored for predicting crime frequency.

The GBR model was chosen as the final prediction model due to its higher accuracy compared to the other models and its ability to handle non-linear relationships in the data.

## Evaluation

Model performance was evaluated using various metrics, including:

*   Accuracy Score
*   Classification Report
*   Confusion Matrix
*   AUC Score (for multiclass classification)
*   R² Score
*   Root Mean Squared Error (RMSE)
*   Mean Absolute Error (MAE)

Cross-validation and hyperparameter tuning were performed to optimize model performance.

## Future Work

Potential future work includes:

*   Saving the best-performing model (GBR) to a pickle file for easy deployment.
*   Deploying the model on a live server using platforms like Azure for real-time crime forecasting and analysis.
*   Exploring more advanced time series forecasting techniques.
*   Incorporating external factors (e.g., weather data, socioeconomic indicators) into the model.

## Conclusion

This project successfully developed and evaluated machine learning models for FBI time series forecasting. The chosen GBR model demonstrated promising results in predicting crime patterns. This project has the potential to contribute to proactive crime prevention and enhance law enforcement efficiency.
