# 🍷 Wine Quality - Exploratory Data Analysis

## Overview
This project performs an exploratory data analysis (EDA) on the WineQT dataset, which contains physicochemical properties of red wine samples along with a quality rating. The goal is to understand the data, identify patterns, and determine which chemical features most influence wine quality.

---

## Dataset
- **Source:** WineQT.csv
- **Rows:** 1143 | **Columns:** 12 (after cleaning)
- **Target Variable:** `quality` — a score from 3 to 8 assigned by wine experts

### Features
| Feature | Description |
|---|---|
| fixed acidity | Most acids in wine that don't evaporate |
| volatile acidity | Amount of acetic acid — too high makes wine taste vinegary |
| citric acid | Adds freshness and flavour to wine |
| residual sugar | Sugar remaining after fermentation |
| chlorides | Amount of salt in wine |
| free sulfur dioxide | Free form of SO₂ — prevents microbial growth |
| total sulfur dioxide | Total amount of SO₂ |
| density | Density of the wine |
| pH | Acidity level (0–14 scale) |
| sulphates | Additive that contributes to SO₂ levels |
| alcohol | Alcohol content percentage |
| quality | Wine quality score (target variable) |

---

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Key Findings
- **Alcohol** is the strongest positive predictor of wine quality (correlation: 0.48)
- **Volatile acidity** is the strongest negative factor — high levels produce a vinegary taste and lower quality scores
- **Citric acid** and **sulphates** have a mild positive influence on quality
- **Density** decreases as quality increases, largely due to its relationship with alcohol content
- The dataset is clean with no missing values, but several features contain outliers that reflect genuine variation in wine samples

---

## EDA Sections
1. Importing Libraries
2. Loading the Data
3. Data Overview & Descriptive Statistics
4. Outlier Detection
5. Correlation Analysis
6. Feature vs Quality Analysis
7. Pairplot of Key Features
8. Conclusion & Next Steps

---

## How to Run
1. Clone the repository
```bash
git clone https://github.com/your-username/wine-quality-eda.git
```
2. Install the required libraries
```bash
pip install pandas numpy matplotlib seaborn
```
3. Open the notebook
```bash
jupyter notebook Wine_Quality_Analysis.ipynb
```
4. Update the dataset path in the loading cell to point to your local `WineQT.csv` file

---

## What's Next
- Build a classification model (Random Forest / Logistic Regression) to predict wine quality
- Handle class imbalance in quality scores
- Engineer new features by combining correlated variables
- Bin quality into Low (3–4), Medium (5–6), High (7–8) for a simpler prediction problem
