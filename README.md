# 💳 Credit Card Default Prediction & Financial Behavior Analysis

## 📊 Project Overview

This project analyzes credit card customer data to detect default patterns and explore customer financial behavior. The aim is to identify **which customers are most likely to default** on their payments and understand the key financial variables that influence this outcome.

This can help financial institutions **minimize risk**, improve **credit scoring models**, and make **data-driven decisions** for managing customer credit limits, payment terms, and collection efforts.

---

## 🧠 Objectives

- Predict the likelihood of a customer defaulting on the next month's payment.
- Understand how **credit limit**, **payment history**, and **bill amounts** relate to defaults.
- Visualize and interpret customer behavior for both defaulters and non-defaulters.
- Provide actionable insights and recommendations based on data.

---

## 📁 Dataset Summary

The dataset includes customer-level information such as:

| Column                   | Description                                      |
|--------------------------|--------------------------------------------------|
| `LIMIT_BAL`              | Credit limit for the customer                    |
| `SEX`, `AGE`, `EDUCATION`, `MARRIAGE` | Demographic information            |
| `PAY_0` to `PAY_6`       | Payment history in the last 6 months            |
| `BILL_AMT1` to `BILL_AMT6` | Outstanding bill amounts for each month        |
| `default payment next month` | Target variable (1 = Default, 0 = No Default) |

---

## 📌 Key Exploratory Analysis

### 🔍 1. **Credit Limit vs Default**
- People with **lower credit limits** are more likely to default.
- As credit limits increase, default risk **decreases**, indicating better financial health and creditworthiness.

### 🔍 2. **Payment History (PAY_0 to PAY_6)**
- Defaulters show **more delayed payments** over several months.
- There’s a strong correlation between payment delays and defaulting behavior.

### 🔍 3. **Outstanding Bill Amounts**
- Customers with **consistently high bills** are more likely to default.
- Defaulting customers tend to maintain **higher outstanding balances** across multiple months.

## 🧮 **Computation Statistics**

### ✅ Why Perform Computational Statistics?

Computational statistics are foundational in data analysis as they help us better understand the structure and behavior of the data before drawing conclusions or building models. Below are the key reasons for using them:

1. **Understand Data Distribution**  
   Computational statistics help uncover how data is distributed — whether it’s skewed, normal, or has outliers.

2. **Measure Spread and Central Tendency**  
   Using the **mean** and **standard deviation**, we can evaluate how concentrated or dispersed the values are around the average.

3. **Apply the Central Limit Theorem (CLT)**  
   CLT allows us to create a sampling distribution from the population. Even if the data is not normally distributed, the distribution of the sample means tends to be normal for sufficiently large sample sizes. This makes statistical inference possible.

4. **Construct Confidence Intervals (CI)**  
   Confidence intervals give us a range in which the population parameter (e.g., mean) is likely to fall. This helps us estimate and reason about data with a quantifiable level of certainty.

5. **Use the t-distribution for Small or Unknown Populations**  
   When the population standard deviation is unknown (common in real-world scenarios), we use the **t-distribution** to make inferences about sample statistics.

---

### 🎯 **Purpose in This Project**

The primary objective of this project is to **identify credit card fraud** or understand **why most users default on their payments**.

Thus, the features selected for computational statistics are **not picked at random**. Instead, they are chosen based on:

- The **business problem** being addressed  
- The **relevance of the variable** to user behavior and financial risk  
- The potential to reveal **insights** about defaulting patterns  

---

### 🔍 Example: `LIMIT_BAL`

In this analysis, the feature **`LIMIT_BAL`** (Credit Limit) was selected to investigate the hypothesis:

> "Are users with lower credit limits more likely to default on their payments?"

By performing statistical analysis on `LIMIT_BAL` for both defaulters and non-defaulters:

- We can construct **confidence intervals** to understand the expected credit limit range for each group.  
- We can apply a **t-test** to determine whether the difference in means is statistically significant.  
- This helps us determine if credit limit is a strong **predictor** of default behavior.  

---

### 📌 Final Note

Performing computational statistics ensures that the insights we derive are **grounded in statistical rigor**, and that any assumptions we make for hypothesis testing or modeling are **justified by the data**.

It sets the stage for deeper **exploratory data analysis** and **predictive modeling**, supporting the project’s goal of uncovering fraud or risky credit behavior.


---

## 📈 Visualizations

A range of plots were used to understand behavior and trends:

- **Line Plot**: shows monthly trend of Bill_1 to Bill_6.

<img src="https://github.com/user-attachments/assets/b6a379ec-dc48-4520-9b80-72d696292d16" height="250"/>

- **Box Plot**: Payment delays across months by defaulters and non-defaulters.

<img src="https://github.com/user-attachments/assets/2b999056-c9e3-4bdf-80c5-de77e7c6882d" height="250"/>

- **Heatmap**: Correlation between billing amounts and default.

<img src="https://github.com/user-attachments/assets/7ddd14ef-3b40-4ef8-a670-c72a0a07241b" height="250"/>

- **Bar Charts**: Monthly average delay per group and bill trends for defaulters.

---

## 📌 Recommendations

- **Monitor customers** with low credit limits and high payment delays more closely.
- Customers with **consistent delays** should trigger early intervention strategies.
- Consider **credit limit adjustments** or payment plans for at-risk clients.
- Use **payment history** as a key input in credit risk modeling.

---

## 🛠️ Tools & Technologies

- **Python** (Pandas, NumPy, Seaborn, Matplotlib)
- **Jupyter Notebook**
- **EDA & Statistical Analysis**
- **Visualization for communication and storytelling**

---

## ✅ Future Improvements

- Build a **machine learning model** (e.g., Logistic Regression, Random Forest) to automate default prediction.
- Include **customer repayment behavior** post-default to improve the lifecycle analysis.
- Integrate **real-time data pipelines** for continuous monitoring.

---

## 📬 Contact

**Developer:** Ronny Muthomi  
**Email:** ronnymuthomi254@gmail.com  
**LinkedIn:** [Ronny M](https://github.com/RonnyMuthomi)  
**GitHub:** [RonnyMuthomi](https://github.com/RonnyMuthomi)

---

> **Note:** This project is for educational purposes and is based on anonymized data.  
