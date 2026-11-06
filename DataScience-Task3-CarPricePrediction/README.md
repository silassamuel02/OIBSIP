# OIBSIP Data Science Internship – Task 3
## Car Price Prediction

### Project Overview
This project builds a machine learning model to predict the selling price of used cars based on vehicle specifications and other details.

### Objective
To analyse used car data, identify important factors affecting car prices, and train regression models to estimate selling prices.

### Dataset
- **Dataset:** Vehicle Dataset from CarDekho
- **File:** `Car details v3.csv`
- **Original records:** 8,128
- **Records after duplicate removal:** 6,926
- **Final modelling records:** 6,923

### Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

### Data Preprocessing
- Removed duplicate records.
- Extracted numeric values from mileage, engine, and maximum power.
- Removed the torque column.
- Handled missing values using median imputation.
- Replaced invalid zero values in mileage and maximum power.
- Removed records with more than 500,000 kilometres driven.
- Applied StandardScaler to numerical features.
- Applied OneHotEncoder to categorical features.

### Exploratory Data Analysis
The analysis explored:
- Selling price distribution.
- Relationship between manufacturing year and selling price.
- Relationship between kilometres driven and selling price.
- Important factors influencing car prices.

### Machine Learning Models
Two regression models were trained and evaluated:

| Model | MAE | RMSE | R² Score |
|---|---:|---:|---:|
| Linear Regression | ₹181,399.77 | ₹339,603.86 | 0.6232 |
| Random Forest Regressor | ₹80,483.19 | ₹164,274.67 | 0.9118 |

### Best Model
Random Forest Regressor achieved the best performance.

- **R² Score:** 91.18%
- **Mean Absolute Error:** ₹80,483.19
- **Root Mean Squared Error:** ₹164,274.67

### Important Features
The most influential features identified by the Random Forest model were:
1. Maximum Power
2. Manufacturing Year
3. Kilometres Driven
4. Mileage
5. Engine Capacity

### Sample Prediction
For a sample car with:
- Year: 2018
- Fuel: Petrol
- Transmission: Manual
- Kilometres Driven: 45,000
- Maximum Power: 82 bhp

The model predicted a selling price of approximately **₹4,72,450**.

### Model Saving
The trained Random Forest pipeline was saved using Joblib as:

`models/car_price_model.pkl`

### Conclusion
The project demonstrates how machine learning regression techniques can estimate used car selling prices. The Random Forest Regressor performed better than Linear Regression on the test dataset, achieving an R² score of approximately 91.18%.

### Repository Structure
```text
DataScience-Task3-CarPricePrediction/
├── car_price_prediction.ipynb
├── Car details v3.csv
├── README.md
└── models/
    └── car_price_model.pkl
```