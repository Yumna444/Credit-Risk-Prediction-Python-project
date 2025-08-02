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

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7dad4870-bd3d-4e94-95d4-a4d0d5058afd" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/62e71b5f-f159-4ed4-b328-0b500019823c" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ee161113-b1b5-4b9e-b318-d99b62490545" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1dc4b081-0472-42fd-8e1e-6434a0a802e8" />

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
