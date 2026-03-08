#HousePrices_KaggleCompetition
House Price Prediction University Competition Winner
Top ranked submission for the Kaggle House Prices: Advanced Regression Techniques competition, built as part of a university data science module me and my partner completed together.
An end to end machine learning pipeline for predicting residential property sale prices. We combined feature engineering, Optuna-tuned ensemble models and a stacked meta-learner to get a competitive RMSE on log-transformed sale prices. Took a while to get the stacking right but really happy with how it turned out.
Custom features derived from the raw dataset include TotalSF (combined floor area), TotalBath, PropertyAge, OverallGrade, QualityArea, and binary amenity flags for pool, basement, fireplace, garage and remodelling. Seperate sklearn pipelines handle categorical and numerical preprocessing via ColumnTransformer. All five base models — Ridge, ElasticNet, KernelRidge, XGBoost, and LightGBM were tuned using Optuna with 150 trials each, then combined through out of fold stacking with a tuned ElasticNet meta learner.
Built with Python, scikit-learn, XGBoost, LightGBM, Optuna, pandas, NumPy and seaborn.

LinkedIn: https://www.linkedin.com/posts/university-american-college-skopje_we-are-proud-to-announce-the-winners-of-the-activity-7409956156028284928-XkVf?utm_source=share&utm_medium=member_desktop&rcm=ACoAAFwagZwBURf5vw5m-Fz2FAdNrPiIDz4XUo8
