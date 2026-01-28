# 🎓 GradeGauge — Student Performance Classification (KNN vs Naive Bayes)

**GradeGauge** is a machine learning notebook project that predicts whether a student is performing **above or below a threshold** using the **StudentsPerformance** dataset.  
It includes a complete workflow: **data loading → exploration → cleaning → feature engineering → scaling → model training → evaluation**.

---

## 📌 What this project does
✅ Loads and explores `StudentsPerformance.csv`  
✅ Checks missing values and dataset structure  
✅ Creates a new feature: **avg_score** (mean of math, reading, writing)  
✅ Builds a binary target:
- `1` if `avg_score > 50`
- `0` if `avg_score <= 50`

✅ Encodes categorical features using **LabelEncoder**  
✅ Splits data into train/test (80/20) with stratification  
✅ Scales features using **StandardScaler**  
✅ Trains and compares two models:
- **K-Nearest Neighbors (KNN)** with **5-fold Cross Validation** to find best `k`
- **Gaussian Naive Bayes** with cross-validation + test evaluation

✅ Evaluates using:
- Accuracy
- Classification report (Precision/Recall/F1)
- Confusion matrix heatmaps

---

## 📁 Notebook
### `OEL.ipynb`
This notebook contains the full pipeline:
1. Data loading + exploration  
2. Feature engineering (`avg_score`, `target`)  
3. Encoding categorical variables  
4. Train/test split + standard scaling  
5. KNN training (CV across multiple k values) + evaluation  
6. Naive Bayes training + evaluation  