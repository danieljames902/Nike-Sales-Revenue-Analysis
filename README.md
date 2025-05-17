# Nike US Sales Revenue Analysis

## Overview
This project predicts Nike's US sales revenue using a Tuned Random Forest model (R²: 0.9840, RMSE: 18,000.59). It includes exploratory data analysis, feature engineering, and actionable recommendations.

## Dataset
**Note**: `Nike_US_Sales.xlsx` is not included due to sensitivity. Place it in `data/` to run the notebook. Contact me at danieljames902@gmail.com for access. Features:
- Units Sold, Operating Profit, Operating Margin
- Retailer ID, Sales Method, Product Name
- Invoice Date (for Year, Month, Quarter)
- Derived: Region, Product Category, Sales_Method_Product_Category

## Methodology
- **EDA**: Revenue trends, correlations, distributions.
- **Feature Engineering**: Region (inferred), Product Category, interaction terms.
- **Modeling**: Tuned Random Forest with RandomizedSearchCV (3-fold StratifiedKFold).

## Results
- **Metrics**: R²: 0.9840, RMSE: 18,000.59, MAE: 7,806.61.
- **Key Drivers**: Units Sold, Operating Profit.
- **High-Revenue Factors**: Online sales, Basketball/Lifestyle, Q4/Q3, West/Northeast.
- **Recommendations**:
  - Boost Units Sold and Online sales.
  - Target Q4/Q3 and West/Northeast regions.
  - Support Southeast (Retailer ID_1197831).

## Repository Structure
- `notebooks/Nike_Sales_Analysis.ipynb`: Full analysis.
- `outputs/feature_importance_features_tuned.png`: Feature importance plot.
- `final_presentation_summary_features_tuned.txt`: Summary.
- `data/`: Place `Nike_US_Sales.xlsx` here (not included).
- `requirements.txt`: Dependencies.
- `scripts/`: Empty.

## How to Run
1. Clone: `git clone https://github.com/danieljames902/Nike-Sales-Revenue-Analysis.git`
2. Install: `pip install -r requirements.txt`
3. Place `Nike_US_Sales.xlsx` in `data/` (contact me for access).
4. Run: `jupyter notebook notebooks/Nike_Sales_Analysis.ipynb`
5. View outputs on Colab.

## Links
- [Portfolio](https://danieljames902.github.io)
- [Interactive Notebook (Colab)](https://colab.research.google.com/drive/17RjXd7y8NdwgicNYqUvyoF3b1o3eIUwI?usp=sharing)