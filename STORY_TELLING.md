# 🏡 Project Title: Price Prediction of Real Estate

---

## ✨ 1. Introduction – Why This Project?

The real estate market is one of the most influential sectors in the global economy. However, accurately pricing a property is a significant challenge, given the wide array of factors influencing it—location, size, crime rate, pollution, accessibility, and more.

In this project, I set out to apply machine learning techniques to predict house prices using real-world data. The ultimate goal is to provide a data-driven tool that supports smarter decisions for homebuyers, sellers, and investors.

---

## 🧾 2. Dataset Overview

- **Source:** Boston Housing Dataset  
- **Records:** 506  
- **Features (13 total):**  
  CRIM (crime rate), ZN (residential land), RM (average rooms), AGE, DIS (distance to employment centers), NOX (pollution), and others.  
- **Target:** MEDV (Median home value in $1000s)

Each row corresponds to a home or tract, and each column represents a feature potentially influencing its price.

---

## 📊 3. Data Exploration – What the Data Tells Us

### 🧠 Key Insights:

- **Price Distribution:** Most houses are priced between $15,000 and $25,000, with a few luxury outliers.
- **RM vs Price:** More rooms generally indicate higher prices.
- **LSTAT:** Strong negative correlation with price—areas with higher lower-status population tend to have lower home values.
- **NOX and CRIM:** Higher pollution and crime rates negatively impact prices.

### 🔍 Visualizations:

- Histogram of home prices  
- Correlation heatmap  
- Boxplots: RM, LSTAT, CRIM vs MEDV  
- Scatter plot: NOX vs MEDV

> _"We discovered that housing prices are highly sensitive to the average number of rooms, environmental pollution, and socioeconomic status."_

---

## 🧠 4. Model Building – Predicting Prices

### 🔬 Models Implemented:

- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor

### 📈 Performance Summary:

| Model                  | Mean Error | Std Dev |
|------------------------|------------|---------|
| Linear Regression      | 4.34       | 1.42    |
| Decision Tree          | 5.67       | 1.75    |
| Random Forest Regressor| 4.34       | 0.89    |

> _"Random Forest outperformed others by offering more consistent and accurate predictions."_

---

## 📌 5. Model Interpretation – What Matters Most?

Using feature importance from the **Random Forest** model (`Evergreen.joblib`), we identified the key factors that most strongly affect house prices.

### 🔝 Top Influential Features:

1. **RM** – Average number of rooms  
2. **LSTAT** – % of lower-status population  
3. **DIS** – Distance to job centers  
4. **CRIM** – Crime rate

> _"Homes with more rooms, situated in low-crime and well-connected neighborhoods, command higher prices."_

---

## 🧠 6. Predictions – How Close Are We?

### Visualizations:

- **Actual vs Predicted Price** – Scatter plot  
- **Error Distribution** – Histogram

> _"Most predictions fall within a ±$3,000 range of actual values, validating the model’s real-world applicability."_

---

## 📌 7. Conclusion – What We Learned

- Real estate prices are affected by a blend of structural, social, and environmental factors.
- Machine learning models—especially ensemble methods like Random Forest—uncover hidden patterns and improve accuracy.
- Data-driven models can significantly empower real estate stakeholders to make informed decisions.

---

## 🔮 8. Recommendations & Future Work

- **Include broader real-world variables** like interest rates, neighborhood facilities, and proximity to schools and hospitals.
- **Deploy the model** as an interactive web dashboard for practical use.
- **Expand** to larger and more diverse datasets for better generalization.

---

📌 _This project serves as a stepping stone to bringing AI into real estate decision-making. With further refinements and data integration, the model can evolve into a robust pricing tool._

