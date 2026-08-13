# 🚗 Car Price Prediction using Machine Learning

## 📌 Project Overview

This project predicts the **selling price of a used car** using Machine Learning.

The model uses car-related features such as:

* Manufacturing year
* Present price
* Kilometres driven
* Fuel type
* Selling type
* Transmission
* Number of previous owners
* Car age

A **Random Forest Regression** algorithm is used to train the model and predict car prices.

---

## 🎯 Objectives

* Analyze car price data using Python.
* Perform data cleaning and preprocessing.
* Perform exploratory data analysis (EDA).
* Create new features using feature engineering.
* Convert categorical data into numerical form.
* Train a regression model.
* Predict car selling prices.
* Evaluate the model using MAE, RMSE, and R² score.
* Understand how Machine Learning can be applied to real-world price prediction.

---

## 📂 Dataset

The project uses a CSV dataset named:

`car data.csv`

### Dataset Features

| Column          | Description                                |
| --------------- | ------------------------------------------ |
| `Car_Name`      | Name of the car                            |
| `Year`          | Manufacturing year                         |
| `Selling_Price` | Selling price of the car — target variable |
| `Present_Price` | Present/ex-showroom price                  |
| `Driven_kms`    | Kilometres driven                          |
| `Fuel_Type`     | Petrol, Diesel, or CNG                     |
| `Selling_type`  | Dealer or Individual                       |
| `Transmission`  | Manual or Automatic                        |
| `Owner`         | Number of previous owners                  |

A new feature called `Car_Age` is created during preprocessing.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**
* **Random Forest Regression**
* **Jupyter Notebook / Google Colab**

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Missing Value Check
   ↓
Duplicate Removal
   ↓
Feature Engineering
   ↓
Exploratory Data Analysis
   ↓
Categorical Encoding
   ↓
Train-Test Split
   ↓
Random Forest Regression
   ↓
Model Training
   ↓
Price Prediction
   ↓
Model Evaluation
   ↓
Visualization
```

---

## 🧹 Data Preprocessing

The following preprocessing steps are performed:

1. Load the CSV dataset using Pandas.
2. Check dataset shape and information.
3. Check for missing values.
4. Remove duplicate records.
5. Create the `Car_Age` feature.
6. Remove `Car_Name` for the basic prediction model.
7. Separate input features (`X`) and target variable (`y`).
8. Encode categorical features using `OneHotEncoder`.

Categorical features:

```text
Fuel_Type
Selling_type
Transmission
```

---

## 🤖 Machine Learning Model

### Random Forest Regression

The project uses `RandomForestRegressor` from Scikit-learn.

```python
RandomForestRegressor(
    n_estimators=300,
    random_state=42
)
```

The dataset is divided into:

* **80% Training Data**
* **20% Testing Data**

The model learns the relationship between car features and selling price and then predicts prices for unseen test data.

---

## 📊 Model Evaluation

The model is evaluated using:

### 1. Mean Absolute Error — MAE

Measures the average difference between actual and predicted prices.

**Lower MAE = Better performance**

### 2. Root Mean Squared Error — RMSE

Measures prediction error while giving more weight to larger errors.

**Lower RMSE = Better performance**

### 3. R² Score

Measures how well the model explains the variation in car prices.

**Higher R² = Better performance**

---

## 📈 Visualizations

The project includes visualizations such as:

* Selling Price Distribution
* Present Price vs Selling Price
* Car Age vs Selling Price
* Actual vs Predicted Selling Prices

These graphs help understand relationships and patterns in the dataset.

---

## 💡 Key Insights

* Present price is an important factor in determining selling price.
* Older cars generally have lower resale values.
* Kilometres driven can influence the resale price.
* Fuel type, transmission, and number of previous owners can affect car value.
* Random Forest Regression can effectively model the relationships between multiple car features and selling price.

---

## 📁 Project Structure

```text
Car-Price-Prediction/
│
├── car data.csv
├── Car_Price_Prediction.ipynb
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Car-Price-Prediction.git
```

### 2. Open the project

```bash
cd Car-Price-Prediction
```

### 3. Install required libraries

```bash
pip install pandas numpy matplotlib scikit-learn
```

### 4. Run the notebook

Open:

```text
Car_Price_Prediction.ipynb
```

Run all cells from top to bottom.

---

## 📦 Requirements

```text
pandas
numpy
matplotlib
scikit-learn
```

---

## 🚀 Future Improvements

The project can be improved by:

* Testing multiple regression algorithms such as Linear Regression, Random Forest, Gradient Boosting, and XGBoost.
* Performing hyperparameter tuning.
* Adding more car-related features.
* Building a web application for real-time price prediction.
* Allowing users to enter car details and receive an estimated selling price.
* Deploying the trained model online.

---

## 🎓 Learning Outcomes

Through this project, I learned:

* Data preprocessing
* Exploratory Data Analysis
* Feature engineering
* Categorical encoding
* Regression Machine Learning
* Random Forest
* Model evaluation
* Data visualization
* Real-world application of Machine Learning

---

## 👨‍💻 Author

**Ajay Ghulghule**

BE Computer Science — Artificial Intelligence & Machine Learning

---

## ⭐ Conclusion

This project demonstrates how Machine Learning can be used to predict used-car prices based on different vehicle characteristics. The complete workflow covers data preprocessing, feature engineering, visualization, model training, prediction, and evaluation.
