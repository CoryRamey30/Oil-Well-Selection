🛢️ Oil Well Selection
📍 Project Overview
OilyGiant has tasked us with identifying the safest and most profitable region to develop 200 new oil wells. Using machine learning and statistical analysis, we evaluated three regions based on their expected profit, oil reserves, and associated risk. Our goal: maximize return while minimizing risk of loss.

💼 Problem Statement
We were given data from three oil-rich regions. Each contains thousands of well samples with reserve volumes and potential production metrics. The challenge is to:

Train models to predict oil production.

Estimate profit from drilling in each region.

Analyze risk using statistical techniques.

Select the top 200 wells per region for profitability.

---

## 🛠 Tools & Technologies Used

- **Python**
- **Pandas** – for data manipulation
- **NumPy** – for numerical operations
- **Matplotlib & Seaborn** – for data visualization
- **Scikit-learn** – for machine learning models (Random Forest, Linear Regression)

---

🔍 Methodology
Data Exploration: Loaded and cleaned the datasets for all three regions.

Modeling: Trained a LinearRegression model for each region.

Evaluation:

Checked R² scores and MSE to measure model accuracy.

Simulated profit using predicted values and region-specific costs.

Risk Analysis:

Performed bootstrap simulations on 500 random samples.

Focused only on the top 200 wells for each simulation.

Calculated the 95% confidence interval for expected profits.

📊 Results Summary
Region 1:

Highest average profit and confidence interval.

Only region with a 95% confidence interval that is always profitable.

Region 0:

Had the highest total reserves (29,601.8), but high variability meant profitability was not guaranteed.

Region 2:

Showed the lowest risk of loss, though with lower average profit.

Interestingly, a simple break-even calculation would suggest none of the regions were profitable — however, by targeting only the top 200 wells, we were able to extract substantial value.

✅ Final Recommendation
Based on average profit, risk of loss, and statistical confidence, we recommend that OilyGiant invest in Region 1 for their next round of well development.
