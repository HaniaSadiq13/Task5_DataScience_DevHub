# Task 5: Personal Loan Acceptance Prediction

## 🎯 Objective
Predict which customers are likely to accept a **personal loan offer** using classification models. This task uses customer attributes to understand and forecast personal loan acceptance behavior.

## 📁 Dataset
- **Name**: Bank Marketing Dataset  
- **Source**: UCI Machine Learning Repository  
- **Target Variable**: `deposit` (yes = accepted loan offer, no = declined)

## 🛠️ Libraries Used
- `pandas`, `numpy` – for data manipulation  
- `matplotlib.pyplot`, `seaborn` – for data visualization  
- `scikit-learn` – for encoding, modeling, and evaluation  

## 🔍 Steps Performed

### 1. Load and Inspect Dataset
- Read the `bank.csv` file using `pandas.read_csv()`
- Checked the shape, column names, and sample data using `.shape`, `.columns`, and `.head()`

### 2. Exploratory Data Analysis (EDA)
- Visualized distributions and counts of:
  - **Age** (Histogram with KDE)
  - **Job** (Count plot)
  - **Marital status**
  - **Target column: deposit**
- Checked for missing values

### 3. Preprocessing
- Categorical columns like `job`, `marital`, `education`, `housing`, etc., were **Label Encoded**
- Target column `deposit` was mapped: `yes → 1`, `no → 0`

### 4. Train-Test Split
- Defined features (`X`) and target (`y`)
- Used `train_test_split()` with 80% training and 20% testing data

### 5. Model Training
- Trained two classifiers:
  - **Logistic Regression**
  - **Decision Tree Classifier**

### 6. Model Evaluation
- Metrics used:
  - **Accuracy Score**
  - **Confusion Matrix**
  - **Classification Report (Precision, Recall, F1)**
- Plotted **Top 10 Important Features** from the Decision Tree model

## 📊 Sample Results

| Model                | Accuracy (example) |
|---------------------|--------------------|
| Logistic Regression | ~88%               |
| Decision Tree       | ~90%               |

## 📌 Key Skills Demonstrated
- ✅ Exploratory Data Analysis  
- ✅ Label Encoding for categorical variables  
- ✅ Classification model training and evaluation  
- ✅ Feature importance analysis  

## 🧠 Business Insight
The model can help identify customer segments (by age, job, marital status, etc.) that are more likely to accept loan offers — improving marketing strategy and campaign targeting.
