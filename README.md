# 🏠 House Price Prediction using Machine Learning

This project builds a complete **Machine Learning pipeline** for predicting California house prices using the **California Housing Dataset**.  
The notebook covers the full workflow from **EDA (Exploratory Data Analysis)** to **model training, evaluation, hyperparameter tuning, and prediction system creation**.

---

## 📌 Project Overview

The goal of this project is to predict the **median house value** based on housing and demographic features such as:

- Longitude
- Latitude
- Housing median age
- Total rooms
- Total bedrooms
- Population
- Households
- Median income
- Ocean proximity

The project demonstrates:

- Data preprocessing
- Data visualization
- Feature engineering pipeline
- Model comparison
- Cross-validation
- Hyperparameter tuning using GridSearchCV
- Final model evaluation
- Predictive inference system

---

## 📂 Dataset

**Dataset:** California Housing Prices Dataset

📎 Kaggle Dataset:  
https://www.kaggle.com/datasets/camnugent/california-housing-prices

The dataset contains housing information collected from California districts.

---

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📊 Workflow

### 1️⃣ Data Loading
- Import dataset using Pandas
- Inspect dataset shape and structure

### 2️⃣ Exploratory Data Analysis (EDA)
- Missing value analysis
- Duplicate row checking
- Statistical summary
- Distribution plots
- Correlation heatmap
- Outlier analysis

### 3️⃣ Data Preprocessing
- Train-test split
- Numerical feature scaling
- Categorical feature encoding
- ColumnTransformer pipeline

### 4️⃣ Baseline Model
A baseline Linear Regression model is trained first.

### 5️⃣ Model Selection
Different regression models are compared using:
- RMSE
- MAE
- R² Score
- K-Fold Cross Validation

Models tested:
- Linear Regression
- Ridge Regression
- Lasso Regression
- Random Forest Regressor
- HistGradientBoostingRegressor

### 6️⃣ Hyperparameter Tuning
GridSearchCV is used to optimize the best model.

### 7️⃣ Final Evaluation
The final tuned model is evaluated on:
- Training data
- Testing data
- Residual analysis

### 8️⃣ Predictive System
A custom prediction function is created for real-world house price prediction.

---

## 🧠 Best Performing Model

✅ **HistGradientBoostingRegressor**

This model achieved the best performance after hyperparameter tuning.

---

## 📈 Evaluation Metrics

The project uses:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score

---

## 📁 Project Structure

```bash
house-price-prediction/
│
├── 15_4_house_price_prediction.ipynb   # Main Jupyter Notebook
├── housing.csv                         # Dataset
├── README.md                           # Project documentation
```

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/house-price-prediction.git
cd house-price-prediction
```

### 2️⃣ Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### 3️⃣ Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook file and run all cells.

---

## 🔍 Key Insights from EDA

- Dataset contains both numerical and categorical features
- `total_bedrooms` contains missing values
- `median_income` has strong positive correlation with house prices
- House prices are capped at higher values in the dataset
- Some numerical features contain outliers

---

## 📌 Future Improvements

- Deploy model using Streamlit or Flask
- Add feature engineering
- Use XGBoost or LightGBM
- Save trained model using Joblib
- Build interactive dashboard

---

## 🎯 Learning Outcomes

This project demonstrates practical understanding of:

- End-to-end machine learning workflow
- Data preprocessing pipelines
- Regression algorithms
- Cross-validation techniques
- Hyperparameter tuning
- Model evaluation

---

## 📜 License

This project is for educational and learning purposes.
