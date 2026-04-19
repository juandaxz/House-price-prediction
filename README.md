# California Housing Price Prediction

This project focuses on building a machine learning model to predict housing prices in California using the California Housing dataset.

The objective is to analyze the data, engineer relevant features, and evaluate different models to estimate median house values based on socio-economic and geographic variables.

## Project Workflow

### 1. Exploratory Data Analysis (EDA)
- Distribution analysis using histograms
- Correlation analysis using heatmaps
- Visualization of relationships between variables
- Geographical analysis using latitude and longitude

### 2. Data Preprocessing
- Handling missing values
- Log transformation applied to reduce skewness
- Encoding categorical variable (ocean_proximity) using one-hot encoding

### 3. Feature Engineering
- Creation of new variables:
  - bedrooms_ratio = total_bedrooms / total_rooms
  - household_rooms = total_rooms / households

### 4. Modeling
The following models were implemented and evaluated:

- Linear Regression
- Random Forest Regressor
- Random Forest with Grid Search

### 5. Evaluation Metrics
- R² Score
- Mean Squared Error (MSE)

## Results

- Linear Regression:
  - R² Score: 0.667
  - MSE: 4450108941

- Random Forest:
  - R² Score: 0.81

- Random Forest (Grid Search):
  - R² Score: 0.74

## Key Insights

- Median income shows strong correlation with house prices.
- Feature engineering improved model performance.
- Random Forest outperformed Linear Regression, indicating non-linear relationships in the data.
- Grid Search did not improve performance, suggesting the need for better hyperparameter tuning.

## Conclusion

This project demonstrates how data preprocessing, feature engineering, and model selection impact predictive performance. Random Forest proved to be the most effective model for capturing complex patterns in the dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn