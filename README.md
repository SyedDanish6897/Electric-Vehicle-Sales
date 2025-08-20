# 📊 Electric Vehicle (EV) Sales Analysis & Prediction in India

## 📌 Project Overview

This project analyzes and predicts **Electric Vehicle (EV) sales across Indian states** using **Data Analysis (DA), Feature Analysis (FA), and Machine Learning (ML)**.
It leverages **state-level EV adoption data** to uncover trends, build predictive models, and support decision-making for **market planning, infrastructure investment, and policy development**.

The notebook covers:

* 🔍 **Exploratory Data Analysis (EDA)** – uncover sales trends by year, month, state, vehicle class & type.
* ⚙️ **Feature Engineering** – extract date features & encode categorical variables.
* 🤖 **Machine Learning Models** – Random Forest Regressor + comparison with other models.
* 📈 **Evaluation & Insights** – feature importance, trend visualizations, and prediction accuracy.


## 📂 Dataset

* **DataSet**: https://drive.google.com/file/d/14_cAtKqyS_nlzAhdhftC7NDlnBx_4YBS/view?usp=sharing
* **Format**: CSV
* **Size**: \~96,800 rows, 8 columns

### Columns:

* `Year` – Year of EV sales
* `Month_Name` – Month of sales
* `Date` – Exact date of sales
* `State` – Indian state / UT
* `Vehicle_Class` – e.g., Sedan, SUV, Bus, etc.
* `Vehicle_Category` – e.g., Commercial, Passenger, Others
* `Vehicle_Type` – e.g., 2-Wheeler, 3-Wheeler, 4-Wheeler
* `EV_Sales_Quantity` – Number of EVs sold


## 🛠️ Tech Stack

* **Programming Language**: Python
* **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
* **Model**: Random Forest Regressor (with scope for XGBoost/LightGBM)
* **Artifacts**: Cleaned dataset (`.parquet`), trained ML model (`.pkl`)

## 🚀 Steps in the Project

1. **Data Collection & Cleaning**

   * Loaded CSV, handled missing values, and converted date columns.

2. **Exploratory Data Analysis (EDA)**

   * Yearly, monthly, and state-wise EV adoption trends.
   * Breakdown by vehicle class, category, and type.

3. **Feature Engineering**

   * Extracted `Year_num`, `Month_num`, `Day_num` from `Date`.
   * Encoded categorical features using **Label Encoding**.

4. **Modeling**

   * Applied **Random Forest Regressor**.
   * Tuned hyperparameters for better performance.

5. **Evaluation**

   * Metrics: MAE, RMSE, R²
   * Example Results:

     json
     {
       "MAE": 11.422,
       "RMSE": 123.25,
       "R2": 0.9417
     }
     
   * Strong predictive power (94% R²).

6. **Visualization**

   * Trends: yearly growth, monthly seasonality, state performance.
   * Feature Importance: identifying key factors driving EV adoption.



## 📊 Key Visuals

* EV Sales by Year
* State-wise EV adoption
* Vehicle Class / Category breakdown
* Actual vs Predicted EV sales scatterplot
* Feature importance (from Random Forest)


## 📦 Installation & Usage

### 1️⃣ Clone Repository

bash
git clone https://github.com/SyedDanish6897/EV-Sales-India.git
cd EV-Sales-India


### 3️⃣ Run Jupyter Notebook

```bash
jupyter notebook EV_Sales_Analysis.ipynb
```


## 📈 Future Improvements

* ✅ Add **XGBoost / LightGBM** models for comparison
* ✅ Build **interactive dashboard** (Streamlit/Flask)
* ✅ Integrate **SQL queries** for deeper state-wise insights
* ✅ Deploy model as an **API service**



## 🧑‍💻 Author

** Syed Danish **

* 💼 Data Analyst | ML Enthusiast
* 🌍 Focus: Data Science, Analytics, and AI Projects
