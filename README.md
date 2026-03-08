# HousePrices_KaggleCompetition


House Price Prediction — University Competition Winner
Top-ranked submission for the Kaggle House Prices: Advanced Regression Techniques competition, built as part of a university data science module.
An end-to-end machine learning pipeline for predicting residential property sale prices, combining rich feature engineering, Optuna-tuned ensemble models, and a stacked meta-learner to achieve a competitive RMSE on log-transformed sale prices.
Custom features derived from the raw dataset include TotalSF (combined floor area), TotalBath, PropertyAge, OverallGrade, QualityArea, and binary amenity flags for pool, basement, fireplace, garage, and remodelling. Separate sklearn pipelines handle categorical and numerical preprocessing via ColumnTransformer. All five base models — Ridge, ElasticNet, KernelRidge, XGBoost, and LightGBM — were tuned using Optuna with 150 trials each, then combined through out-of-fold stacking with a tuned ElasticNet meta-learner.
Built with Python, scikit-learn, XGBoost, LightGBM, Optuna, pandas, NumPy, and seaborn.
