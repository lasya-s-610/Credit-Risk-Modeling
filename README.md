# Credit-Risk-Modeling
## 🧠 Objective  
The goal of this project is to predict whether a person’s credit score will **increase**, **decrease**, or **stable** based on their income, expenses, and personal details. This can help banks or financial companies better understand customer behavior and reduce financial risk.

---

## 📊 Dataset Creation  
We created a **realistic synthetic dataset** with 25,000 records. Each record represents a person with features such as Age, Location, Gender, Monthly Income, EMI payments, Credit Utilization Ratio, etc.

Values were generated with realistic distributions and location-based ranges gathered from publicly available sources. For example, people in metropolitan areas had higher average incomes and older age profiles.

| Feature           | Metropolitan      | Urban            | Semi-Urban       | Rural            |
|-------------------|-------------------|------------------|------------------|------------------|
| **Average Age**   | 28                | 30               | 29               | 26               |
| **Age Range**     | 21–60             | 20–65            | 18–60            | 15–58            |
| **Gender Ratio**  | 3:1 → 75% M       | 5:2 → 71% M      | 2:1 → 67% M      | 5:4 → 56% M      |
| **Average Income**| ₹1.5L             | ₹90k–₹1L         | ₹50k–₹75k        | ₹20k–₹25k        |
| **Income Range**  | ₹15k–₹5L          | ₹10k–₹4L         | ₹8k–₹2.5L        | ₹5k–₹2L          |

---

## ⚙️ Preprocessing and Modeling  
- Removed outliers  
- Performed label encoding for categorical features (e.g., Gender, Location)  
- Used **SMOTE** (Synthetic Minority Oversampling Technique) on the training data to handle class imbalance  
- Trained multiple models: **Logistic Regression**, **Decision Tree**, and **Random Forest**  
- **Decision Tree** was chosen due to its superior performance on imbalanced data  
- Used **GridSearchCV** for hyperparameter tuning

---

## 📈 Model Results  
- **Accuracy:** 97.9%  
- **F1 Score:** 98.07%  
- The "Stable" class was the most frequent, and SMOTE + tuning helped ensure balanced performance across all classes

---

## 💡 Business Insights  
This model helps identify **credit behavior patterns** across various customer segments based on income, repayment history, and credit usage:

- Most people’s credit scores remain **stable**, as expected.
- Banks can proactively identify **risky customers** and improve offerings for **low-risk** and **stable** users.

---

## 🏦 Product or Policy Recommendations  

**1. High-Risk Customers:**  
- Offer flexible repayment plans  
- Temporarily lower credit card limits  
- Limit loan offerings until behavior improves  

**2. Stable Customers:**  
- Provide quick access to personal loans or credit cards  
- Recommend safe financial products  
- Reward consistent repayment behavior annually  

**3. Low-Risk Customers:**  
- Increase credit limits or reduce interest rates  
- Encourage long-term savings through special plans  
- Introduce "Buy Now, Pay Later" options  
- Reward major credit milestones with vouchers  

---

## 📁 Project Files  
- `credit_data.csv` – Full synthetic dataset  
- `Lasya_credit_project.ipynb` – Main project code notebook (modeling + insights)

---

## 📝 Author  
**Lasya**

---
