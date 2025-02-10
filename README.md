# Air Quality Prediction

## Overview
This project aims to predict air quality using machine learning techniques. The dataset includes various environmental attributes, and the model predicts the relative humidity (`RH`). The project implements data preprocessing, feature engineering, hyperparameter tuning, and model evaluation.

## Features
- **Data Preprocessing:** Handles missing values, removes highly correlated features, and converts date & time formats.
- **Feature Scaling:** Standardizes features using `StandardScaler`.
- **Model Selection:** Implements `RandomForestRegressor`, `LGBMRegressor`, and `StackingRegressor`.
- **Hyperparameter Tuning:** Uses `Optuna` for optimizing model parameters.
- **Model Evaluation:** Assesses performance using `R²`, `MAE`, and `RMSE`.
- **Visualizations:** Includes prediction error histogram and scatter plot of actual vs. predicted values.

## Dataset
The dataset is loaded from a CSV file and includes attributes such as:
- `Date`, `Time`
- `CO`, `NO2`, `O3`, `SO2`, etc.
- `RH` (Target variable: Relative Humidity)

## Installation
To run this project, install the required dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn optuna lightgbm
```

## Usage
Run the Jupyter Notebook to execute the analysis:
```bash
jupyter notebook airquality.ipynb
```


## Results
- **Cross-Validation R² Mean:** Shows model performance on training data.
- **Optimized Stacking Model R²:** Measures accuracy on test data.
- **MAE & RMSE:** Evaluate prediction errors.
- **Visualizations:**
  - Histogram of prediction errors
  - Scatter plot of actual vs. predicted values

## Contributions
Feel free to contribute by optimizing the model further, adding new features, or improving visualizations.

## License
This project is open-source and available under the MIT License.

