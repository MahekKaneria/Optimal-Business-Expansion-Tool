# ProfitMax: Optimal Store Location Predictor

## Project Information

**Project Name:** ProfitMax: Optimal Store Location Predictor
**GitHub Repository**: Optimal-Business-Expansion-Tool
**Prepared by:** Mahek Kaneria  

---

## Project Overview
**ProfitMax** is a data-driven solution designed to assist businesses in identifying the most profitable locations for store expansion. By leveraging store performance data, demographic features, and operational costs, this tool predicts optimal locations to maximize revenue and profitability. The project combines machine learning models with feature engineering to recommend locations with the highest potential profit margins.The goal is to provide a data-driven approach to optimize store locations based on key factors such as traffic busyness, median income, and operational costs, allowing for informed decision-making in store expansion.

---

## Key Objectives

- **Predict Annual Revenue**: Use features like traffic busyness index, median income, and operational costs to predict the annual revenue of potential new store locations.
- **Estimate Profit Margins**: Calculate estimated profit margins by subtracting operational costs from predicted revenues.
- **Recommend Locations**: Identify the top locations with the highest predicted profit margins for opening new stores.

---

## Files Included

- **store_data.csv**: Dataset containing information about the sales, operational costs, and other details of existing stores.
- **survey_combined.xlsx**: Dataset containing information about potential store locations, including traffic busyness index, expected operational costs, and other demographics.
- **store_location_analysis.ipynb**: A Jupyter Notebook file containing the entire analysis process, including data exploration, feature engineering, model building, prediction, location recommendation and visualizations.


---

## Libraries Used

The following Python libraries were utilized in this project for data analysis, machine learning, and visualization:

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical computing and array handling.
- **Matplotlib**: For data visualization.
- **Scikit-learn**: For machine learning and model evaluation.
- **XGBoost**: For building the machine learning model to predict store profitability.
- **TensorFlow**: For experimenting with neural network models (though XGBoost was selected as the final model).
- **GridSearchCV**: For hyperparameter tuning and model optimization.

---

## Important Information

- **Data Sources**: The data used in this project, including `store_data.csv` and `survey_combined.xlsx`, is fictional and designed for the purpose of this analysis.
- **Objective**: To recommend optimal store locations for Cire Coffee Co. using a data-driven approach.
- **Machine Learning Methods**: XGBoost was selected based on its performance in predicting annual revenue, with the model achieving an R² value of ~0.74. TensorFlow was also evaluated but did not perform as well.

---

## Steps Performed

### 1. Data Exploration
- Examined the distribution of key variables such as annual revenue and profit margins.
- Explored the correlation between traffic busyness, median income, and store profitability.

### 2. Feature Engineering
- Standardized key features such as median income, traffic busyness index, and operational costs.

### 3. Model Building and Prediction
- Built and evaluated two machine learning models (XGBoost and TensorFlow) to predict annual revenue based on existing store data.
- XGBoost was selected due to better performance (MSE: 954M, R²: 0.748).
- Applied the trained XGBoost model to predict potential revenue for new store locations.
- Calculated the estimated profit margin for each location by subtracting operational costs from predicted revenue.

### 4. Location Recommendation
- Identified the top 10 locations based on predicted profit margins, providing data-driven insights for store expansion.

---

## Visualization

- **Feature Importance**: Displayed feature importance scores from the XGBoost model to understand which factors contribute most to the predictions.
- **Predicted vs Actual Revenue**: A scatter plot comparing predicted vs actual revenues for model validation.
- **Aggregate Comparison**: Compared the aggregate revenue and profit margin for the top 10 locations (as predicted by the model) against randomly selected locations.
- **Profit Margin Distribution**: A histogram showing the distribution of predicted profit margins for the surveyed locations.

---

## Results

The top 10 locations predicted to yield the highest profit margins were identified, with **Sunstannell** being the most promising. The tool provides a clear comparison of potential revenue and costs across different locations, offering actionable insights for business expansion.

## Next Steps

- Further on-ground research may be conducted for the recommended locations.
- The current model can be iteratively improved with more data or additional feature engineering.
- The same approach can be extended to other areas or industries that require location-based decision-making.

---

## Conclusion

ProfitMax is a comprehensive tool designed to assist businesses in making data-driven decisions for store expansion. By using machine learning to predict optimal store locations, businesses can minimize risk and maximize profitability, ensuring successful expansion strategies.
