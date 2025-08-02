# Credit Risk Prediction

## 📌 Objective
This project aims to predict whether a loan applicant is likely to default or not (Risk_Flag: 1 or 0) based on various customer attributes. This helps financial institutions make informed lending decisions.

---

## 📊 Dataset
**Dataset Used:** Credit Risk Dataset  
**Source:** Provided during the internship (or specify if it's from Kaggle, UCI, etc.)  
**Target Variable:** `Risk_Flag`  
**Features:**
- Id
- Income
- Age
- Experience
- Married/Single
- House_Ownership
- Car_Ownership
- Profession
- CITY
- STATE
- CURRENT_JOB_YRS
- CURRENT_HOUSE_YRS

---

## 🧰 Tools and Technologies Used
- Python (Jupyter Notebook - Anaconda)
- Pandas, NumPy (Data Handling)
- Seaborn, Matplotlib (Visualization)
- Scikit-learn (Machine Learning & Evaluation)

---

## 🔄 Workflow Summary

### 📂 Step 1: Data Loading
- Loaded the dataset using Pandas.
- Explored the data with `.info()`, `.describe()`, and `.isnull().sum()`.


### 🧹 Step 2: Data Cleaning
- Checked and confirmed no missing values.
- Removed `Id` column (not useful for prediction).
- Verified data types.

### 🔤 Step 3: Categorical Encoding
- Used **Label Encoding** for:
  - `Married/Single`
  - `House_Ownership`
  - `Car_Ownership`
  - `Profession`
  - `CITY`
  - `STATE`

### 📊 Step 4: Exploratory Data Analysis (EDA)
- Plotted:
  - Income distribution
  - Risk vs Income boxplot
  - Risk vs Age
  - Gender vs Credit Risk (fixed as 'Married/Single')
- Checked data balance with `Risk_Flag.value_counts()`

### 🧠 Step 5: Model Building
- Features: All except `Risk_Flag`
- Target: `Risk_Flag`
- Train-Test Split: 80-20
- Used **Random Forest Classifier**

### 📈 Step 6: Model Evaluation
- **Accuracy:** ~54.5%
- **Confusion Matrix:**

📊 Visualizations
Income Distribution

Risk Flag vs Income

Risk Flag vs Age

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/293b71b2-487c-4904-b18f-cdc60f442f64" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/100e28b3-3e70-44bf-a3ae-25c547d6ccc4" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e0e328e2-f49f-4825-8b7c-93a4c89a38ef" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f09661ff-8abf-4aa6-8fd7-7c37660bddf4" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5266c10a-9025-4a74-bc43-131803f520e5" />


✅ Conclusion
While the Random Forest model showed moderate accuracy (~54%), the results indicate the need for:

Feature selection

Handling class imbalance

Hyperparameter tuning

Trying other models like XGBoost or LightGBM

This project is a strong starting point for improving risk assessment models in the financial sector.


Files in This Repo
credit_risk_prediction.ipynb – Main notebook

README.md – Project documentation
excel file of data set
