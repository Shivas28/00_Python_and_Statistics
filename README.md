# 🐍 Python & Statistics Foundations

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)

> Core Python programming, data manipulation with Pandas, exploratory data analysis, and statistical inference — the foundation behind every ML project in this portfolio.

---

## 📚 Notebooks

# 🐍 1. Python Basics I — Core Programming Exercises

## 📌 Overview
Fundamental Python programming exercises covering control flow, loops, and real-world logic problems.

## 🔍 What's Inside
- Prime number checker using loop and `for-else`
- Random number product quiz using `random` module
- Squares of even numbers in range 100–200
- Hospital Billing System — room charges, lab tests, medicine, 10% discount logic

## 🛠️ Libraries
`random`

---

# 🐍 2. Python Basics II — Data Structures & NumPy

## 📌 Overview
Hands-on practice with Python's core data structures and an introduction to NumPy arrays and Pandas DataFrames.

## 🔍 What's Inside
- List operations — `append`, `extend`, `insert`, `remove`, `pop`, `sort`, `reverse`, `clear`
- Tuple immutability demonstration with explanation
- Set deduplication behavior
- Dictionary — create, update, add new keys
- Voting eligibility and grade checker using conditionals
- NumPy — scalar, 1D array, 2D array (2×3), random 4×4 integer matrix
- Pandas DataFrame — `info()`, `describe()`, column selection, drop, fillna, drop duplicates

## 🛠️ Libraries
`numpy` `pandas`

---

# 📊 3. Basic Statistics — Sales Data Analysis

## 📌 Overview
Statistical analysis of sales data covering central tendency, spread, and distribution using visualizations.

## 📂 Dataset
- **File:** `sales_data_with_discounts.csv`
- **Features:** Avg Price, Total Sales Value, Discount Rate, Net Sales Value, Volume, Brand, City, BU

## 🔍 What's Inside
- Summary statistics table — Mean, Median, Mode, Std Dev, Min, Max
- Histograms for all numerical columns
- Boxplots — outlier identification across sales features
- Bar charts for categorical columns (Brand, City, BU, Model)
- Insight: Mean > Median → data is right-skewed, driven by large transactions

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn`

---

# 🏥 4. Pandas Data Wrangling — Hospital Billing

## 📌 Overview
Real-world data wrangling on hospital patient and billing records using Pandas merge, groupby, and concat operations.

## 📂 Dataset
- **Files:** `Patient_Data.csv`, `Billing_Data.csv`

## 🔍 What's Inside
- Column selection and duplicate removal by `PatientID`
- Missing `BillAmount` imputed with column mean
- `groupby` — total revenue per department (Cardiology highest at ₹11,200)
- `merge` on `PatientID` — joining patient and billing tables
- `concat` — adding new week's patient records
- Final merged DataFrame with `InsuranceCovered` and `FinalAmount`

## 🛠️ Libraries
`pandas`

---

# 🫀 5. EDA — Cardiotocographic Fetal Health Data

## 📌 Overview
Exploratory data analysis on fetal heart rate monitoring data, focusing on outlier treatment and feature relationships with health outcomes.

## 📂 Dataset
- **File:** `Cardiotocographic.csv`
- **Target:** `NSP` (1 = Normal, 2 = Suspect, 3 = Pathologic)

## 🔍 What's Inside
- Missing value imputation with column means
- Outlier detection and capping using IQR method (before/after boxplots)
- Summary stats table — Mean, Median, Std Dev, IQR per feature
- Histograms for LB, ASTV, MSTV, Width
- NSP class frequency bar chart
- Correlation heatmap across all features
- Violin plot — ASTV distribution across NSP categories

## 📊 Key Insight
> Higher ASTV → more likely Suspect or Pathologic. Lower AC → worse NSP outcome.

## 🛠️ Libraries
`pandas` `numpy` `matplotlib` `seaborn`

---

# 📐 6. Confidence Intervals — Print Head Durability

## 📌 Overview
Constructs 99% confidence intervals using both t-distribution (unknown population std) and z-distribution (known population std) on a small sample of print head durability data.

## 🔍 What's Inside
- Sample of n=15 print head lifetimes
- **t-distribution CI** — used because n < 30 and population std unknown
  - t-critical (df=14, 99%) = 2.977
  - 99% CI: **1.090 to 1.387** million characters
- **z-distribution CI** — used when population std = 0.2 is known
  - z-critical = 2.576
  - 99% CI: **1.106 to 1.372** million characters
- Business conclusion: company can guarantee ~1.1M character lifespan

## 🛠️ Libraries
`numpy` `scipy`

---

# 🧪 7. Hypothesis Testing — Weekly Cost Analysis

## 📌 Overview
One-tailed z-test to determine whether restaurant weekly costs have exceeded the theoretical model prediction of ₹4,000.

## 🔍 What's Inside
- H₀: μ = 4000 (model is correct)
- H₁: μ > 4000 (costs have risen)
- Sample mean = 3050, σ = 125, n = 25
- z-calculated = -38.0 → far below critical value (1.645)
- p-value = 1.0 → **Fail to reject H₀**
- Conclusion: no evidence costs exceeded model; sample mean actually much lower

## 🛠️ Libraries
`scipy` `math`

---

## 📊 Topics Covered

| Topic | Notebook |
|-------|----------|
| Python Core Programming | `01_Python_Basics_I.ipynb` |
| Data Structures & NumPy | `02_Python_Basics_II.ipynb` |
| Descriptive Statistics | `03_Basic_Stats_Sales.ipynb` |
| Pandas Data Wrangling | `04_Pandas_Hospital_Data.ipynb` |
| Exploratory Data Analysis | `05_EDA_Cardiotocographic.ipynb` |
| Confidence Intervals | `06_Confidence_Intervals.ipynb` |
| Hypothesis Testing | `07_Hypothesis_Testing.ipynb` |

---

## 🛠️ How to Run

```bash
# Clone the repo
git clone https://github.com/Shivas28/ML-Portfolio.git

# Navigate to folder
cd ML-Portfolio/00_Python_and_Statistics

# Launch Jupyter
jupyter notebook
```

---

## 👨‍💻 Author

**SHIVAS** — [GitHub](https://github.com/Shivas28)

> ⭐ If you find this useful, please star the repo!
