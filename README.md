# eda_with_python
# Task 5: Exploratory Data Analysis (EDA) - Titanic Dataset

## 📌 Objective
Perform Exploratory Data Analysis on the Titanic dataset to uncover patterns, trends, and relationships between passenger attributes and survival rates.

**Tools Used:**
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📂 Dataset
**Source:** [Titanic Dataset - Kaggle](https://www.kaggle.com/c/titanic)  
**Files used:**
- `train.csv` — Passenger data with survival labels.

**Key Columns:**
- `Survived` (0 = No, 1 = Yes)
- `Pclass` — Ticket class (1, 2, 3)
- `Sex` — Gender
- `Age` — Age in years
- `SibSp` — Number of siblings/spouses aboard
- `Parch` — Number of parents/children aboard
- `Fare` — Ticket fare
- `Embarked` — Port of embarkation

---

## 🛠 Steps Performed
1. **Data Loading & Inspection**
   - Loaded `train.csv` using Pandas.
   - Checked data types, missing values, and statistical summary.

2. **Data Cleaning**
   - Filled missing `Embarked` values with mode.
   - Filled missing `Age` values with median.
   - Created `Has_Cabin` flag for cabin availability.

3. **Univariate Analysis**
   - Histograms and boxplots for numeric columns (`Age`, `Fare`).
   - Countplots for categorical columns (`Sex`, `Pclass`, `Embarked`).

4. **Bivariate Analysis**
   - Survival rate by `Sex`, `Pclass`, and `Age`.
   - Fare distribution among survivors and non-survivors.

5. **Correlation Analysis**
   - Generated correlation heatmap.
   - Pairplot for selected numeric features.

6. **Feature Engineering**
   - Created `FamilySize` and `IsAlone`.
   - Extracted `Title` from `Name` and grouped rare titles.

7. **Observations & Summary**
   - Females had higher survival rates than males.
   - First-class passengers survived more often than third-class.
   - Children had higher survival rates.
   - Higher fares and cabin availability were associated with survival.

---

## 📊 Key Insights
- **Overall survival rate:** ~38%
- **By Sex:** Female ~74%, Male ~19%
- **By Class:** 1st ~63%, 2nd ~47%, 3rd ~24%
- Passengers paying higher fares generally had better survival chances.
- Traveling alone reduced survival likelihood.

---

## 📁 Deliverables
- `EDA_Titanic.ipynb` — Jupyter Notebook with full analysis and visualizations.
- `analysis_graphs.docx` (and other saved plots).

---

