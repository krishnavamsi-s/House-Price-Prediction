# 🏠 House Price Prediction Web App

This is a complete end-to-end data science project that predicts California house prices using a Random Forest model. The project includes data collection, preprocessing, model training, evaluation, visualization, and a deployed web interface built with Flask and Tailwind CSS.

---

## 📁 Project Structure

├── app.py # Main Python Flask app

├── model.pkl # Trained RandomForest model (generated after first run)

├── scaler.pkl # Scaler used for normalization (generated)

├── static/

│ ├── feature_importance.png # Bar plot of feature importances

│ └── actual_vs_predicted.png # Scatter plot of true vs predicted values

├── templates/

│ └── index.html # Frontend HTML (Tailwind CSS form and plots)

└── README.md # This file

---

## 📊 Dataset Used

- **Source**: `fetch_california_housing()` from Scikit-learn
- **Target**: `MedHouseVal` — Median house value in $100,000s
- **Features**:
  - `MedInc`: Median income in block
  - `HouseAge`: Median house age
  - `AveRooms`: Average rooms per household
  - `AveBedrms`: Average bedrooms per household
  - `Population`: Block population
  - `AveOccup`: Average household occupancy
  - `Latitude`, `Longitude`

---

## ⚙️ Technologies Used

- Python
- Scikit-learn
- Flask (for web API)
- Tailwind CSS (for styling)
- Matplotlib & Seaborn (for plots)
- Joblib (for saving models)

---


## 🌐 Web Interface

- Enter house parameters like income, age, rooms, population, etc.
- Click **Predict** to get the estimated house price.
- The interface displays two key visualizations:
  - 📊 **Feature Importance**: A bar chart showing the influence of each feature on the prediction.
  - 📈 **Actual vs Predicted**: A scatter plot comparing the model’s predictions to actual values.

---

## 🧠 Model Details

- **Model**: `RandomForestRegressor` with 100 decision trees
- **Preprocessing**: `StandardScaler` for normalizing input features
- **Evaluation Metrics**:
  - **MSE**: Mean Squared Error — measures average squared difference between actual and predicted values.
  - **R² Score**: Coefficient of Determination — measures how well future samples are likely to be predicted.


