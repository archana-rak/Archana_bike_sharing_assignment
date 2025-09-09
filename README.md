# 🚴‍♂️ BoomBikes Demand Prediction – Multiple Linear Regression  

## 📌 Problem Statement  
BoomBikes, a US-based bike-sharing provider, faced a significant revenue decline during the COVID-19 pandemic. To recover and prepare for future growth, the company wants to **understand the factors affecting bike rental demand**.  

The objective is to build a **Multiple Linear Regression model** that predicts bike rental demand (`cnt`) based on various independent variables like weather conditions, season, holidays, and year.  

---

## 🎯 Business Goal  
- Identify **significant variables** affecting bike demand.  
- Understand how well these variables explain demand variations.  
- Help BoomBikes **strategize pricing and supply planning** in a post-pandemic market.  

---

## 📂 Dataset  
The dataset contains daily bike rental demand data along with factors like:  
- **`season`** (spring, summer, fall, winter)  
- **`yr`** (0 = 2018, 1 = 2019)  
- **`weathersit`** (clear, cloudy, light rain, heavy rain)  
- **`holiday`**, **`workingday`**, **`temp`**, **`hum`**, **`windspeed`**  
- **`casual`**, **`registered`**, and **`cnt`** (total demand)  

Target Variable:  
- **`cnt`** = Total bike rentals (casual + registered)  

👉 Note: Some numeric categorical variables like `season` and `weathersit` were converted to categorical strings before modeling.  

---

## 🛠️ Methodology  
1. **Data Preparation & Cleaning**  
   - Checked missing values, outliers, and feature encoding.  
   - Converted categorical variables into dummy variables.  

2. **Exploratory Data Analysis (EDA)**  
   - Studied patterns in demand across seasons, weather, holidays, and working days.  

3. **Model Building**  
   - Built a **Multiple Linear Regression** model.  
   - Performed feature selection using **RFE (Recursive Feature Elimination)**.  
   - Compared **Ridge** and **Lasso Regularization** to handle multicollinearity.  

4. **Model Evaluation**  
   - Evaluated model using **R² score** on training and test sets.  
   - Residual analysis to validate assumptions.  

---

## 📊 Results  
- Identified that **year, temperature, and season** significantly impact bike demand.  
- Higher demand observed in **2019 compared to 2018**, showing growth trend.  
- Weather conditions and humidity negatively affect demand.  
- Final model achieved strong **R² score on test data** (close to training score, indicating generalization).  

---
