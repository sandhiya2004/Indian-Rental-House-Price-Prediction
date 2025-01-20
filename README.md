# Indian Rental House Price Prediction

## Overview

This project predicts rental house prices in Indian cities like Delhi, Mumbai, and Pune using machine learning. The model uses house characteristics and location data to provide accurate price estimates.

## Features

- **House Type**: Apartment, Villa, etc.
- **House Size**: Area in square feet.
- **Location**: Specific areas within cities.
- **City**: Delhi, Mumbai, Pune.
- **Price**: Target variable.
- **Other Attributes**: Number of bathrooms, balconies, status (furnished/unfurnished).

## Project Workflow

1. **Data Preparation**:
   - Combine city datasets.
   - Handle missing values and engineer features.
2. **Exploratory Data Analysis (EDA)**:
   - Visualize trends and detect outliers.
   - Analyze relationships between features and price.
3. **Feature Selection**:
   - Identify key predictors using Lasso regression.
4. **Model Training**:
   - Train multiple regression models: Linear, Ridge, Decision Tree, Random Forest, XGBoost, and KNN.
   - Evaluate using metrics: MAE, RMSE, and R² Score.

## Results

- **Best Model**: XGBoost Regressor
  - Test R² Score: **0.9736**
  - Key hyperparameters (GridSearchCV):
    - `colsample_bytree`: 0.8, `gamma`: 0, `learning_rate`: 0.1, `max_depth`: 7, `n_estimators`: 300, `subsample`: 0.8.
- Other top-performing models:
  - Random Forest (R² Score: 0.9703)
  - K-Neighbors Regressor (R² Score: 0.9639)

## Directory Structure

```
project_root/
|-- data/
|   |-- Indian_housing_Delhi_data.csv
|   |-- Indian_housing_Mumbai_data.csv
|   |-- Indian_housing_Pune_data.csv
|-- end-to-end-indian-rental-houseing-price-prediction.ipynb
|-- requirements.txt
|-- README.md
```

## How to Run

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the script:
   ```bash
   python main.py
   ```
3. Review results and visualizations.

## Future Enhancements

- Add more city data.
- Explore deep learning models.



## Contact

For queries, reach out to [Sandhiya K] at [[kssandhiya23@gmail.com](mailto\:kssandhiya23@gmail.com)].

