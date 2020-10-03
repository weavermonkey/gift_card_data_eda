# Predicting gift card transactions
## Insights
1. Steady growth in transactions.
2. Sharp peaks in December, dips in January.
3. Weekly seasonality in data.

## Feature engineering
1. Convert date string to timestamp.
2. Moving averages of transaction - 7,14,21,28 day windows.
3. Lag - previous 6 values.
4. 'Growth' - monotonically increasing integer.
5. One hot encoding for month and weekend.

## Modeling
1. Linear regression, lasso, and ridge
2. MLP
3. Random forest
4. SVR
5. KNN

Plot predictions, perform hyperparameter tuning on models with low prediction error.

**random forest, lasso, and ridge had >90% accuracy**

## Recommendation
Either lasso or ridge, depending on how accurate feature importance is.

## Scope for improvements.
 - Additional features based on business inputs.
 - LSTM for forecasting.
 - Retrain after removing features with low importance.
 - Make 'Growth' variable more accurate.