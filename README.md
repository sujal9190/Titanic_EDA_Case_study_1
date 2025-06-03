# 🚢 Titanic Dataset - Exploratory Data Analysis (EDA)

This project performs an in-depth **Exploratory Data Analysis (EDA)** on the classic Titanic dataset. The objective is to understand the key patterns, relationships, and data quality issues that influence passenger survival.

---

## 📌 Data Description

| Column Name   | Description                                                                |
| ------------- | -------------------------------------------------------------------------- |
| `survived`    | Survival (0 = No, 1 = Yes) – **target variable**                           |
| `pclass`      | Passenger class (1 = First, 2 = Second, 3 = Third)                         |
| `sex`         | Gender of the passenger (`male` or `female`)                               |
| `age`         | Age of the passenger (in years)                                            |
| `sibsp`       | Number of siblings/spouses aboard the Titanic                              |
| `parch`       | Number of parents/children aboard the Titanic                              |
| `fare`        | Fare paid for the ticket                                                   |
| `embarked`    | Port of embarkation (`C` = Cherbourg, `Q` = Queenstown, `S` = Southampton) |
| `class`       | Duplicate of `pclass` but as a string (`First`, `Second`, `Third`)         |
| `who`         | Broad categorization: `man`, `woman`, or `child`                           |
| `adult_male`  | Boolean indicating whether the passenger is an adult male                  |
| `deck`        | Deck level (A–G or NaN if unknown)                                         |
| `embark_town` | Full name of the embarkation town                                          |
| `alive`       | Duplicate of `survived`, but as `yes` or `no`                              |
| `alone`       | Boolean indicating whether the passenger was alone (no family aboard)      |

---

## 📌 Project Objectives

- Load and inspect the Titanic dataset.
- Perform univariate and bivariate analysis.
- Identify and treat outliers.
- Analyze data skewness and kurtosis.
- Visualize feature relationships.
- Prepare data for modeling or reporting.

---

## 📊 Dataset Overview

The dataset contains passenger information from the Titanic shipwreck, including:

- **Survival status** (0 = No, 1 = Yes)
- **Passenger class (Pclass)**
- **Age, Gender, Fare**
- **Siblings/Spouses aboard (SibSp)**
- **Parents/Children aboard (Parch)**

---

## 🛠️ Key Libraries Used

- `pandas` – Data manipulation
- `numpy` – Numerical operations
- `seaborn` & `matplotlib` – Visualization
- `scipy.stats` – Skewness & kurtosis analysis

---

## 🔍 Exploratory Analysis Performed

### ✅ 1. Data Cleaning
- Checked for missing values.
- Converted data types where needed.

### ✅ 2. Univariate Analysis
- Histograms and value counts for numerical and categorical variables.
- Distribution plots for skewed features.

### ✅ 3. Bivariate Analysis
- Survival rates by class, sex, and age group.
- Pairplots for numeric features with `hue='Survived'`.

### ✅ 4. Outlier Detection & Treatment
- IQR method used to detect outliers.
- Outliers replaced with median values for stability.

### ✅ 5. Skewness & Kurtosis
- Skewness and kurtosis calculated for all numerical features.
- Transformations suggested (e.g., log/sqrt) where needed.

---

## 📈 Sample Visualizations

- Pairplot of numerical features by survival status
- Boxplots of Fare and Age by survival
- Count plots for categorical distributions

> 📸 All visualizations are created using `seaborn` and `matplotlib`.

---

## 📁 File Structure

```bash
EDA_case_1.ipynb    # Jupyter notebook with complete EDA workflow
Titanic.csv         # Dataset file
README.md           # Project overview (this file)
