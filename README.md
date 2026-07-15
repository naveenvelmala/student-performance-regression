# Student Performance Prediction — Linear Regression, Ridge & Lasso

Predicting a student's **Performance Index** (continuous target) from study habits, using
Linear Regression, Ridge, and Lasso regression, with a comparison of accuracy and coefficients.

## Dataset
[Student Performance (Multiple Linear Regression)](https://www.kaggle.com/datasets/nikhil7280/student-performance-multiple-linear-regression) — 10,000 student records with:
- `Hours Studied`
- `Previous Scores`
- `Extracurricular Activities` (Yes/No)
- `Sleep Hours`
- `Sample Question Papers Practiced`
- `Performance Index` (target, 10–100)

## Approach
1. Load and inspect the data (nulls, dtypes, correlations)
2. Encode `Extracurricular Activities` as 0/1
3. Train/test split (80/20)
4. Scale features with `StandardScaler`
5. Train Linear Regression, Ridge (alpha=1.0), and Lasso (alpha=0.1)
6. Evaluate each with MAE, MSE, RMSE, and R²
7. Compare coefficients across the three models
8. Conclude which model generalizes best and why

## Results
See `Student_Performance_Regression_.ipynb` for the full comparison table and coefficient plot.

## How to run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook Student_Performance_Regression_.ipynb
```
Make sure `Student_Performance.csv` (downloaded from Kaggle) is in the same folder as the notebook.

## Tools
Python, pandas, scikit-learn, matplotlib, seaborn
