# 📊 E-commerce Marketing Mix Modeling (MMM)

This project runs a full-cycle Marketing Mix Modeling for an e-commerce business using synthetic data covering 3 years of monthly marketing and sales metrics. It includes data exploration, feature engineering, model building, multicollinearity analysis, and actionable business insights.

---

##  Overview

-  **Dataset**: 3 years (36 months) of monthly e-commerce marketing and sales data
-  **Goal**: Understand the impact of various marketing channels and business factors on sales performance
-  **Model**: Linear Regression (with options to extend to Ridge/Lasso)
-  **Key Features**: TV, Digital, Email, Influencer Spend, Discount, Price, Holiday Season, Web Traffic
-  **Metrics Used**: R², MAE, RMSE, VIF (for multicollinearity), and Coefficient calculations

---

##  Project Structure

```
📂 ecom-mmm/
│
├── 3_year_marketing_data.csv         # Synthetic data file
├── mmm_analysis.ipynb                # Google Colab Notebook with full MMM workflow
├── README.md                         # Project documentation (this file)
└── images/                           # Folder for visualizations
```

---

##  Key Steps

### 1. Data Preparation
- Cleaned and structured synthetic data
- Feature engineering: Total_Marketing_Spend, Total_Marketing_ROI, Effective_Price

### 2. Model Building
- Linear Regression using `scikit-learn`
- Evaluation: R², RMSE, MAE
- Visualization: regplots, residuals, coefficient tables

### 3. Multicollinearity Check
- Calculated Variance Inflation Factor (VIF)
- Removed redundant features like `Total_Marketing_Spend` and `Paid_Traffic`

### 4. Insights & Recommendations
- Identified high-impact features (e.g., Holiday_Season, Promo_Discount)
- Suggested marketing budget reallocation based on respective impacts
- Explained price sensitivity using regression coefficients

---

##  Sample Visualization

![image](https://github.com/user-attachments/assets/56f1b9e6-e368-4c91-adf5-c4adc9495f49)
  
```python
sns.regplot(x='Total_Marketing_Spend', y='Total_Marketing_ROI', data=data)
```

---

##  Business Recommendations

- Increase budget during **Holiday Seasons** to maximize ROI
- Optimize **discount strategy** rather than blanket promotions
- Improve **Digital Marketing ROI** through campaign audits
- Expand **Email Campaigns** for better personalization and engagement

---

##  Tech Stack required

- Python 3.10+
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Statsmodels (for VIF and diagnostics)

---

> Feel free to fork this repo, add enhancements, or create a pull request. Feedback is always welcome!


> Made with ❤️ by Swaroop Gaddam  
📧 swaroop.gaddam01@gmail.com  
🌐 https://www.linkedin.com/in/swaroop-gaddam/

