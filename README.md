# House Price Prediction: Advanced Regression Model - Build during Data Scientist at Milestone PLM Solutions Pvt. Ltd., Thane

[![GitHub stars](https://img.shields.io/github/stars/yourusername/house-price-prediction?style=social)](https://github.com/abubakarpungiwale/house-price-prediction/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/yourusername/house-price-prediction?style=social)](https://github.com/abubakarpungiwale/house-price-prediction/network)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Project Overview

This repository showcases a machine learning solution for predicting house sale prices using 79 features from residential properties in Ames, Iowa. Developed during a Data Scientist internship at Milestone PLM Solutions Pvt. Ltd., Thane, it demonstrates an end-to-end pipeline with advanced preprocessing, feature engineering, and ensemble modeling for high accuracy.

**Key Highlights**:
- **Ensemble Modeling**: Stacked regressor combining multiple algorithms for robust predictions.
- **Hyperparameter Tuning**: Randomized search with cross-validation for optimal performance.
- **Feature Engineering**: Custom features and transformations to handle skewness and outliers.

## Table of Contents

- [Project Overview](#project-overview)
- [Key Technologies](#key-technologies)
- [Installation](#installation)
- [Methodology](#methodology)
- [Performance Metrics](#performance-metrics)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Key Technologies

- **Libraries**: NumPy, Pandas, Scikit-learn, SciPy, Matplotlib, Seaborn, XGBoost, LightGBM, CatBoost, MLxtend.
- **Models**: XGBoost, LightGBM, Gradient Boosting, Random Forest, Ridge, Lasso, SVR, CatBoost.
- **Ensemble**: Stacking with Ridge meta-regressor.
- **Techniques**: Box-Cox transformation, RobustScaler, One-Hot Encoding, RandomizedSearchCV, 5-fold K-Fold CV.
- **Metric**: RMSE on log-transformed prices.

## Installation

```bash
git clone https://github.com/abubakarpungiwale/house-price-prediction.git
cd house-price-prediction
pip install -r requirements.txt
```

## Methodology

- **Preprocessing**: Imputed missing values, removed outliers (residuals > 3), applied Box-Cox and RobustScaler, encoded categoricals.
- **Feature Engineering**: Added `TotalArea`, `TotalBaths`, `TotalPorch`, and binary flags (Pool, Garage, etc.).
- **Training**: Tuned 8 models with RandomizedSearchCV, used 5-fold CV.
- **Ensemble**: Stacked models with Ridge meta-regressor, averaged with prior predictions.

## Performance Metrics

- **Training**: Mean CV RMSE ≈ **0.115** (5-fold), indicating strong generalization.
- **Test**: Estimated RMSE ≈ **0.12** on test set (top 10% in competitive evaluation).
- **Insights**: Ensemble reduced errors by 5-10% vs. individual models. Visualizations in notebook enhance interpretability.

## Contributing

Fork and submit pull requests for enhancements.

## License

MIT License - see [LICENSE](LICENSE).

## Contact

- **Author**: Abubakar Maulani Pungiwale
- **Email**: abubakarp496@email.com
- **LinkedIn**: [linkedin.com/in/abubakarpungiwale](https://linkedin.com/in/abubakarpungiwale)
- **Contact**: +91 9321782858

Reach out for ML project discussions or data science opportunities!
