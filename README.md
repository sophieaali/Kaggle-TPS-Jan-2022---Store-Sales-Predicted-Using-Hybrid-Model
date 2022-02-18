# Kaggle-TPS-Jan-2022---Store-Sales-Predicted-Using-Hybrid-Model

The dataset used for this notebook is from https://www.kaggle.com/c/tabular-playground-series-jan-2021

"Linear regression excels at extrapolating trends, but can't learn interactions. XGBoost excels at learning interactions, but can't extrapolate trends." - Hybrid model method take from kaggle course: https://www.kaggle.com/ryanholbrook/hybrid-models

In this notebook, I am using Linear Regression to fit the original target series, then using the second algorithm (XGBoost) to fit the residual series. This process is using LR to extrapolate the trend, transform the target to remove the trend, then apply XGBoost to the detrended residuals.

Results of the hybrid model are in the last cell of this notebook
