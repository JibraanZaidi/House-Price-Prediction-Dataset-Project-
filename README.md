# 🏡 House Price Prediction - Data Preprocessing

## 📌 Project Overview

This project focuses on **data preprocessing** for a house price prediction dataset. The dataset is cleaned, preprocessed, and augmented to ensure high-quality inputs for a machine learning model.

## 📂 Dataset Information

- **Source:** Kaggle
- **File Used:** `train.csv`
- **Features:** Various attributes related to house prices, such as `MSSubClass`, `LotFrontage`, `OverallQual`, etc.
- **Target Variable:** `SalePrice`

## 🛠 Steps Performed

### 1️⃣ Data Loading 💅

- The dataset is loaded using `pandas.read_csv()`.
- Initial exploration with `df.shape`, `df.info()`, and `df.describe()`.
- Viewing sample rows using `df.head()`, `df.tail()`, and `df.sample()`.

### 2️⃣ Data Cleaning 🧩

- **Handling Missing Values:**
  - Identified using `df.isnull().sum()`.
  - Removed missing values using `df.dropna()`.
- **Removing Duplicates:**
  - Identified using `df.duplicated().sum()`.
  - Removed using `df.drop_duplicates()`.

### 3️⃣ Data Preprocessing 🛠

- **Categorical Encoding:**
  - Used `LabelEncoder()` to convert categorical columns into numerical values.
- **Feature Scaling:**
  - Applied `StandardScaler()` to normalize numerical columns.

### 4️⃣ Data Visualization 📊

- Used Pandas plotting functions to analyze distributions:
  - `bar`, `barh`, `pie`, `density` plots for categorical features.

### 5️⃣ Data Augmentation 🌱 (If Applied)

- Synthetic data generation through transformations.

### 6️⃣ Saving the Processed Data 💾

- Saved the cleaned dataset using `df.to_csv('cleaned_data.csv', index=False)`.

