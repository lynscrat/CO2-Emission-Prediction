# CO2-Emission-Prediction
Exploratory data analysis and modeling on CO₂ emissions data to understand the impact of various factors on emission levels. Includes preprocessing, visualization, and model evaluation.

### Project Overview
This project analyzes a dataset of CO2 emissions from various vehicles. The primary goal is to predict CO2 emissions based on vehicle specifications. The project involves data exploration, preprocessing, feature engineering, and the implementation and evaluation of several machine learning models.

### 🧭 Objectives
- Perform exploratory data analysis (EDA) on vehicle emission data.
- Compare regression models to identify the best-performing one.

### 🧩 Data Preprocessing
- Features were standardized for consistent scaling.
- Feature correlations were examined to detect multicollinearity.

During the analysis, it was found that several features were highly correlated, causing multicollinearity. This problem can distort regression coefficients and reduce the interpretability and stability of linear models.

To address this issue, two approaches were tested:
1. Variance Inflation Factor (VIF) Reduction
   - Features with VIF values greater than 10 were removed.
   - This reduced redundancy but also removed some potentially informative features.
2. Principal Component Analysis (PCA)
   - PCA was applied to transform correlated variables into uncorrelated components.
   - This preserved more information while resolving multicollinearity.
  
✅ Result:
The PCA-based approach produced better model performance compared to simply dropping high-VIF features.


