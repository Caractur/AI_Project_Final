# Impact of AI on Digital Media (2020–2025) — Regression Project

This repository analyzes the **Global AI Content Impact Dataset** and builds a **Linear Regression** model to predict **“Revenue Increase Due to AI (%)”**. It includes data exploration, preprocessing, model training/evaluation, and experiment logging with MLflow.

## 📦 Files

- `AI_Finalfr.ipynb` — Jupyter notebook with the full workflow.
- `README.md` — You're reading it.

## 🔄 Workflow

1. **Data Access**
   - Downloaded via `kagglehub` (`atharvasoundankar/impact-of-ai-on-digital-media-2020-2025`).
   - Loaded into pandas.

2. **Exploratory Data Analysis**
   - Boxplots for numeric features.
   - Pie charts for categorical distributions.
   - Correlation heatmap.

3. **Preprocessing**
   - Select numeric columns.
   - Standardize with `StandardScaler` using `ColumnTransformer`.

4. **Modeling**
   - Train/test split with scikit-learn.
   - **LinearRegression** model fit on scaled features.

5. **Evaluation**
   - Metrics: **R²**, **RMSE**, **MAE**.
   - Scatter plot of Actual vs. Predicted values.

6. **Experiment Tracking & Artifacts**
   - MLflow logs: params, metrics, model.
   - Model saved via `joblib`.

7. **Export**
   - Predicted target column added back to a CSV copy.

## ▶️ How to Run

# 1. Clone
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

# 2. (Optional) Create & activate a virtual env
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate

# 3. Install deps
pip install -r requirements.txt
# or
pip install pandas numpy matplotlib seaborn scikit-learn kagglehub mlflow joblib

# Open the notebook
jupyter notebook AI_Finalfr.ipynb

# Requirements 
pandas
numpy
matplotlib
seaborn
scikit-learn
kagglehub
mlflow
joblib


