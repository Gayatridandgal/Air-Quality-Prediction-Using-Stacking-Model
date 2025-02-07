# Air Quality Prediction Using Stacking Model

## 📌 Project Overview
This project focuses on predicting relative humidity (RH) using an optimized **Stacking Model** combining **Random Forest** and **LightGBM** regressors. The dataset consists of air quality measurements, and we employ **feature selection, hyperparameter tuning, and visualization** techniques to improve model performance.

## 🚀 Features & Optimizations
- **Data Preprocessing**
  - Handling missing values and outliers
  - Feature scaling using StandardScaler
  - Removing highly correlated features
- **Model Training & Optimization**
  - Stacking model with **Random Forest & LightGBM**
  - **Optuna for hyperparameter tuning** (reduced trials for faster execution)
  - **Cross-validation with KFold (3 splits)** for robust evaluation
  - **Parallel processing (`n_jobs=-1`)** to speed up computations
- **Performance Metrics**
  - R² Score
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
- **Visualizations**
  - Error distribution plot
  - Actual vs. Predicted values scatter plot

## 📊 Dataset
- **Source**: [Kaggle - Air Quality Data](https://www.kaggle.com/datasets)
- **Preprocessing Steps**:
  - Converted Date and Time columns
  - Dropped irrelevant and highly correlated columns
  - Normalized numerical features
  - Used **30% of dataset** for faster model execution

## 🛠️ Tech Stack
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Optuna, LightGBM)
- **Machine Learning** (Stacking Regressor, Hyperparameter Optimization, Feature Engineering)

## 📌 Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/Gayatridandgal/air-quality-prediction.git
   cd air-quality-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the script:
   ```bash
   python main.py
   ```

## 📌 Future Improvements
- Add more advanced feature engineering
- Experiment with additional models like **XGBoost or CatBoost**
- Deploy model using **Flask or FastAPI**



