# **Credit Risk Analysis & Loan Default Insights**

## **Project Overview**
Banks issue thousands of loans, but not every borrower repays on time. Identifying **high-risk borrowers** early helps financial institutions reduce financial losses and improve lending strategies.

This project analyzes loan applicant data to **identify credit risk patterns and understand factors contributing to loan defaults**. An **interactive Power BI dashboard** was built to help banks monitor portfolio performance and detect risky borrower segments.

**Project Goals**
- **Predict which loan applicants may default**
- **Understand risk in the bank’s loan portfolio**
- **Identify borrower segments with higher default probability**
- **Support better data-driven lending decisions**



## **Business Problem**
Banks need to clearly understand:

- **How many loans are issued**
- **How many borrowers fail to repay (defaults)**
- **Which types of customers are high risk**
- **Which loan categories have higher default probability**

Without proper analysis, banks may approve loans to **high-risk borrowers**, increasing financial losses.

This dashboard helps banks **analyze loan performance and identify risky lending segments.**



## **Dataset**
Source: **Kaggle – Credit Risk Dataset**

**Dataset Size**
- **32,581 rows**
- **13 columns**

The dataset contains borrower demographics, financial attributes, loan information, credit history, and loan repayment status.  
These variables help analyze **credit risk patterns and borrower repayment behavior**.



## **Data Cleaning & Analysis (Python)**

Data preprocessing and exploratory analysis were performed using **Python**.

### **Steps**

**1. Load Dataset**
- Import dataset using Python libraries.

**2. Data Cleaning**
- Checked and corrected **data types**
- Converted categorical features to **category data type**
- Encoded historical default indicator to numeric values
- Identified **missing values**

**Handling Missing Data**
- Missing values in employment length and interest rate were filled using **median values**
- Median was used because it **reduces the impact of extreme values and outliers**

**3. Exploratory Data Analysis (EDA)**
- Analyzed **loan default vs non-default distribution**
- Performed **univariate analysis for numerical features**
- Generated **correlation heatmap** to understand feature relationships
- Analyzed **default percentage across loan grades and loan purposes**

**4. Save Cleaned Dataset**
- Cleaned dataset exported for use in **Power BI dashboard**



## **Tools Used**

- **Python** – Data cleaning and analysis  
- **Pandas & NumPy** – Data manipulation  
- **Matplotlib & Seaborn** – Exploratory visualizations  
- **Power BI** – Interactive dashboard and reporting  
- **DAX** – Measures and calculated metrics



# **Power BI Dashboard**

A **three-page interactive dashboard** was developed to analyze loan performance and borrower risk.


## **1. Loan Portfolio Overview**

### **Goal**
Understand the **overall health of the bank’s loan portfolio.**

### **Key Insights from this Page**
- Total number of **loan applications**
- Total **loan amount issued**
- **Average interest rate**
- **Percentage of loan defaults**
- Most common **loan purposes**

### **Business Question**
**“Is the bank’s loan portfolio healthy?”**

This page provides a **high-level summary of lending performance.**


## **2. Risk Analysis**

### **Goal**
Identify **high-risk borrower segments**.

### **Key Insights from this Page**
- Which **loan grades have the highest default rates**
- How **home ownership affects loan risk**
- How **loan purpose influences default probability**
- Relationship between **income and loan amount**

### **Risk Segmentation Logic**

Green → Default Rate < 15% (Low Risk)

Yellow → Default Rate 15–25% (Moderate Risk)

Red → Default Rate > 25% (High Risk)

### **Business Question**
**“Which borrowers are more likely to default?”**

This page helps banks **detect risky lending segments before approving loans.**



## **3. Customer & Financial Insights**

### **Goal**
Understand **borrower behavior and financial patterns.**

### **Key Insights from this Page**
- Which loan purposes are most common
- How interest rates vary across borrower segments
- Distribution of loan amounts
- Borrower demographic patterns

### **Business Question**
**“Which loan types generate the most demand and potential revenue?”**

This page helps banks improve **loan product strategy and pricing decisions.**



# **Key Insights**

- **Lower income borrowers with higher loan amounts show higher default risk**
- **Lower credit grade borrowers have significantly higher default rates**
- Some loan purposes have **higher risk compared to others**
- **Income stability and employment length influence repayment ability**



# **Business Impact**

This project helps financial institutions:

- **Identify high-risk borrowers**
- **Improve credit risk evaluation**
- **Reduce loan defaults**
- **Make data-driven lending decisions**
- **Optimize loan approval strategies**


# **Screenshots**

![Dashboard Screenshot](https://github.com/VibhaCodes/Bank-Loan-Analysis-Dashboard/blob/0a54a0e294e657d1d1d571829a274c8d57d7d6fc/Overview%20Page.PNG)

![Dashboard Screenshot](https://github.com/VibhaCodes/Bank-Loan-Analysis-Dashboard/blob/0a54a0e294e657d1d1d571829a274c8d57d7d6fc/Loan%20Risk%20Analysis.PNG)

![Dashboard Screenshot](https://github.com/VibhaCodes/Bank-Loan-Analysis-Dashboard/blob/0a54a0e294e657d1d1d571829a274c8d57d7d6fc/Customer%20Insights.PNG)
