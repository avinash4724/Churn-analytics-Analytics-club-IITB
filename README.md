# Churn-analytics-Analytics-club-IITB

Project IITB analytics club, churn prediction

# Customer Churn Analytics & EDA

## Project Goal
Reduce **monthly churn rate by 15%** over a simulated **3-month period** by:
- Identifying key churn drivers
- Segmenting customers
- Recommending targeted retention strategies based on data-driven insights


## Project Deliverables
1. **Cleaned Master Dataset** (`cleaned_master.csv`)  
   - Standardized column names  
   - Merged demographic, activity, and subscription datasets  
   - Engineered features (recency, tenure, watch activity, etc.)  

2. **ML-Ready Dataset** (`ml_ready.csv`)  
   - One-hot encoded categorical variables  
   - Standardized numerical features  

3. **Exploratory Data Analysis (EDA)**
   - Correlation heatmap for numeric features  
   - Distributions of activity and subscription metrics  
   - Churn rate by plan, device, location, age group, content preference, billing cycle  
   - Summary statistics and key insights  

4. **Visual Outputs**  
   - All plots saved in `plots/` folder  
   - Inline plots in Jupyter Notebook  

## Process Overview
1. **Data Cleaning**  
   - Standardized columns across datasets using synonym resolution  
   - Removed duplicates and handled missing values with median/mode imputation  

2. **Feature Engineering**  
   - Aggregated user-level metrics from activity logs  
   - Calculated `recency_days`, `tenure_days`, `avg_watch_per_active_day`  
   - Created `churn_label` target variable  

3. **EDA & Insights**  
   - Churn rate patterns by customer segments  
   - Usage behavior analysis and feature importance exploration  
   - Key drivers identified for potential retention actions  

## Future Prospects
To extend this project:
- **Predictive Churn Model:** Implement Logistic Regression, Decision Tree, or Random Forest to predict churn probability for each customer.
- **Customer Segmentation:** Use clustering (e.g., K-Means) to group customers by behavior for targeted retention strategies.
- **Retention Strategy Simulation:** Model impact of different intervention strategies to measure potential churn reduction.

## 🛠 Tech Stack
- **Languages:** Python 3.x  
- **Libraries:** pandas, numpy, matplotlib, seaborn, scikit-learn  
- **Tools:** Jupyter Notebook, Excel/CSV  


##  Usage
1. Place the three raw datasets into the `data/` folder:
   - `customer_churn_data.xlsx`
   - `demographic_data.csv`
   - `subscription_payment_history.csv`
2. Run the provided `churn_eda_feature_engineering.ipynb`
3. Access outputs in:
   - `cleaned_master.csv`
   - `ml_ready.csv`
   - `plots/` folder for visualizations


