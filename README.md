# 🏠 House Price Prediction using Machine Learning

A Machine Learning project that predicts house prices based on property features such as area, number of bedrooms, bathrooms, stories, parking spaces, and furnishing status. The project covers data preprocessing, exploratory data analysis (EDA), feature engineering, model building, and evaluation.

---

## 📌 Project Overview

- **Type:** Regression Problem
- **Dataset:** [Housing.csv](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset) (Kaggle) — 545 rows, 13 columns
- **Target Variable:** `price`
- **Models Compared:** Linear Regression, Decision Tree Regressor, Random Forest Regressor

## 📂 Repository Structure

```


## 🗺️ Roadmap / Phases

| Phase | Description |
|---|---|
| 1 | Problem Understanding |
| 2 | Dataset Collection & Understanding |
| 3 | Data Cleaning & Preprocessing |
| 4 | Exploratory Data Analysis (EDA) |
| 5 | Feature Engineering |
| 6 | Model Building |
| 7 | Model Evaluation |
| 8 | Conclusion & Future Scope |

## 📊 Dataset Features

| Feature | Description |
|---|---|
| area | Plot/house area in sq. ft. |
| bedrooms | Number of bedrooms |
| bathrooms | Number of bathrooms |
| stories | Number of floors |
| mainroad | On main road (yes/no) |
| guestroom | Has guest room (yes/no) |
| basement | Has basement (yes/no) |
| hotwaterheating | Has hot water heating (yes/no) |
| airconditioning | Has AC (yes/no) |
| parking | Number of parking spots |
| prefarea | In preferred area (yes/no) |
| furnishingstatus | furnished / semi-furnished / unfurnished |

## 🔍 Exploratory Data Analysis

The `charts/` folder contains 9 EDA visualizations:
1. Price distribution histogram
2. Price outliers box plot
3. Correlation heatmap
4. Area vs Price scatter plot
5. Bedrooms vs Price scatter plot
6. Furnishing status count plot
7. Main road access count plot
8. Pair plot of key numeric features
9. Average price by furnishing status bar chart

## 🤖 Model Performance

| Model | MAE | RMSE | R² Score |
|---|---|---|---|
| **Linear Regression** | 970,043 | 1,324,507 | **0.653** |
| Random Forest Regressor | 1,022,545 | 1,403,779 | 0.610 |
| Decision Tree Regressor | 1,226,190 | 1,610,551 | 0.487 |

**Linear Regression performed best.** With a dataset of this size (~545 rows) and fairly linear feature-price relationships, the simpler model generalized better than the tree-based models.

**Top price drivers (Linear Regression coefficients):** bathrooms, air conditioning, hot water heating, and preferred area location.

## 🔮 Future Scope

- Use a larger dataset for more reliable predictions
- Add location-based features (city/locality, distance to city center, amenities)
- Try advanced models (XGBoost, Gradient Boosting) with hyperparameter tuning
- Build a web app (Streamlit/Flask) for live price prediction
- Deploy the model as an API

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
