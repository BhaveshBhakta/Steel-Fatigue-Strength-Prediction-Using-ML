## Steel Fatigue Strength Prediction

### Project Overview

This project aims to predict the **fatigue strength of steel** based on its processing parameters and chemical composition. By analyzing a dataset of various thermal treatments, temperature, and material properties, the goal is to develop a regression model that can accurately forecast the fatigue strength. This is a critical task in materials science and mechanical engineering, as it helps in designing durable and safe components.

-----

### Technical Highlights

  * **Dataset**: [Kaggle - Steel Fatigue Strength Prediction](https://www.kaggle.com/datasets/chaozhuang/steel-fatigue-strength-prediction)
  * **Size**: 437 entries, 27 columns
  * **Key Features**:
      * **Thermal Treatment**: `NT`, `THT`, `THt`, `THQCr`, `CT`, `Ct`, `DT`, `Dt`, `QmT`, `TT`, `Tt`, `TCr`.
      * **Chemical Composition**: `C`, `Si`, `Mn`, `P`, `S`, `Ni`, `Cr`, `Cu`, `Mo`.
      * **Other**: `RedRatio`, `dA`, `dB`, `dC`.
  * **Approach**:
      * **Data Cleaning**: The dataset was clean with no missing values or duplicates. The `Sl. No.` column was not used.
      * **Exploratory Data Analysis**: Histograms and a heatmap were used for visualization to understand data distributions and correlations.
      * **Regression Task**: The target variable is `Fatigue`.
      * **Models Used**:
          * A suite of regression models were trained, including Ridge, XGBoost, Random Forest, AdaBoost, Gradient Boosting, Bagging, Decision Tree, SVR, and K-Nearest Neighbors (KNN).
  * **Best R² Score**:
      * **0.988** with XGBoost Regressor.
      * **0.974** with Random Forest Regressor and Gradient Boosting Regressor.
      * The very high R² scores indicate that the models are highly effective at predicting steel fatigue strength based on the provided material properties and processing parameters.

-----

### Purpose and Applications

  * Enable engineers and materials scientists to **predict the fatigue strength of steel** without extensive physical testing.
  * Optimize manufacturing processes for steel to improve its durability and lifespan.
  * Support data-driven decision-making in the design of critical components for civil, mechanical, and aerospace engineering.
  * Provide a foundational model for materials informatics and property prediction.

-----

### Installation

Clone the repository:

```bash
git clone https://github.com/BhaveshBhakta/Steel-Fatigue-Strength-Prediction-Using-ML.git
cd Steel-Fatigue-Strength-Prediction-Using-ML
```

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Performing comprehensive hyperparameter tuning and cross-validation for the top-performing regression models.
  * Exploring more advanced feature engineering, such as creating new features from the chemical composition ratios.
  * Investigating alternative scaling methods or outlier handling strategies.
  * Adding explainability (e.g., SHAP or LIME) to understand which material and processing parameters are the most significant drivers of fatigue strength.
