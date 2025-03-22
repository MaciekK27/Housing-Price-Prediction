# 🏠 Housing Price Prediction
## 📌 Project Overview
This project predicts housing prices using machine learning models like Random Forest and XGBoost. The Jupyter Notebook (housing_prediction.ipynb) includes:
- ✔️ **Data exploration & preprocessing**
- ✔️ **Feature engineering**
- ✔️ **Model training and evaluation**
- ✔️ **Visualizations**

## 📂 Dataset Information
- **Source**: `Housing.csv` (not included; add your own dataset)  
- **Features**:  
  - *Numerical*: `area`, `bedrooms`, `bathrooms`, `stories`, `parking`  
  - *Binary*: `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`  
  - *Categorical*: `furnishingstatus` (one-hot encoded)  
- **Target**: `price` (log-transformed as `log_price`)  
- **Size**: 545 entries, no missing values

## ⚙️ Requirements
Install the required Python libraries:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib
```

## 🚀 How to Use This Project
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/MaciekK27/housing-price-prediction.git
cd housing-price-prediction
```
### 2️⃣ Add the Dataset
Copy Housing.csv into the project folder
### 3️⃣ Open and Run the Jupyter Notebook
```bash
jupyter notebook housing_prediction.ipynb
```

## 📊 Results
- 📈 **R² Score**: 0.671  
- 📉 **RMSE/Mean Price**: 26.7%
 
## 📁 Project Files
- housing_prediction.ipynb → Main notebook (data analysis, training, evaluation)
- images/ → Graphs & plots (e.g., raw_price_skewness.png)
- models/best_xgb_model.pkl → Saved XGBoost model

## 📈 Visualizations
### Price Distribution (Before & After Log Transform)
- `raw_price_skewness.png` → Shows skewness in original prices and how log transformation helps.
### Feature Importance (XGBoost)
- `feature_importance.png` → Reveals which features drive predictions most.
### Predicted vs. Actual Prices
- `predicted_vs_actual.png` → Compares model predictions to real prices.
### Residual Plot
- `residual_plot.png` → Displays the spread of prediction errors.

## 🛠 Possible Improvements
- 🔹 Try other models (LightGBM, CatBoost, ANN)
- 🔹 Perform feature selection for better generalization
- 🔹 Deploy model as an API using Flask/FastAPI
- 🔹 Experiment with hyperparameter tuning

## 📬 Contact
- 📧 **Email**: maciejkrawczynski2727@gmail.com
- 🔗 **GitHub**: [MaciekK27](https://github.com/MaciekK27)
