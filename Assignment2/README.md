# Assignment 2: Hypothesis Testing and Visualization using t-tests

## 📌 Objective
The goal of this assignment is to understand and apply **t-tests** for hypothesis testing.  
We perform:
- **One-Sample t-test** → Compare one group’s mean against a known/hypothetical value.  
- **Two-Sample Independent t-test** → Compare means of two groups to check if they are significantly different.  
- Apply t-test on a **Churn Dataset** to check if customer churn depends on certain attributes (e.g., MonthlyCharges).  

Visualization is used to support the statistical test results.  

---

## 📊 Dataset
1. **Sample Dataset (Numpy Arrays)**  
   - Group A and Group B exam scores (manually created arrays).  
   - Used for practicing one-sample and two-sample t-tests.  

2. **Churn Dataset (Telco Customer Churn)**  
   - *Columns used:*  
     - `Churn` → Whether customer left (1) or stayed (0).  
     - `MonthlyCharges` → Customer’s monthly bill amount.  
   - Split into two groups:  
     - Churned customers (Churn=1)  
     - Non-churned customers (Churn=0)  

---

## 🔎 Steps I Followed
1. **Practice with Sample Dataset**
   - Created two numpy arrays (Group A & Group B).
   - Performed **One-Sample t-test**:
     - Checked if mean of Group A is different from 80.  
   - Performed **Two-Sample t-test**:
     - Compared Group A vs Group B means.  
   - Visualized results using **Histogram (one-sample)** and **Boxplot (two-sample)**.  

2. **Churn Dataset Analysis**
   - Loaded dataset and encoded `Churn` column (Yes=1, No=0).  
   - Selected attribute **MonthlyCharges**.  
   - Split dataset into two groups: Churned vs Non-Churned.  
   - Performed **Two-Sample t-test** to check if average monthly charges differ significantly.  
   - Visualized results using:
     - **Boxplot** (Churn vs MonthlyCharges).  
     - **Histogram** (distribution of monthly charges by churn status).  

3. **Interpretation**
   - Used **t-statistic and p-value** to judge significance.  
   - If *p < 0.05* → Attribute has significant impact on churn.  
   - If *p > 0.05* → No significant difference.  

---

## 📈 Results
- **One-Sample t-test (Group A vs mean=80):**  
  - Found whether Group A’s average significantly differed from 80.  

- **Two-Sample t-test (Group A vs Group B):**  
  - Showed if the two groups’ means were significantly different.  

- **Churn Dataset (MonthlyCharges vs Churn):**  
  - Customers who churned had **higher average monthly charges**.  
  - p-value < 0.05 → MonthlyCharges has a significant effect on churn.  
  - Visualizations supported this conclusion.  

---

## 📝 Learning
- Understood the difference between **one-sample** and **two-sample t-tests**.  
- Learned how to interpret **t-statistic** and **p-value**.  
- Saw how **visualization (boxplots, histograms)** makes hypothesis testing results more intuitive.  
- Connected hypothesis testing with real-world datasets (Churn analysis).  

---

## ⚡ Conclusion
- **t-tests** help in checking whether group differences are *real* or just *random chance*.  
- In the churn dataset, **MonthlyCharges significantly influence churn** → higher charges lead to more churn.  
- Visualizations (histograms, boxplots) made it easy to **see differences** between groups.  
- This assignment strengthened understanding of combining **statistics + visualization** in data analysis.  
