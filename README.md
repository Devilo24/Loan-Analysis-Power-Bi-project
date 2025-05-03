
# 📊 Loan Default Analysis Dashboard – Power BI

This personal project is built to explore and analyze loan default patterns from a financial dataset containing over 250,000 records. The data was ingested from a local SQL Server database using **Power BI Dataflow Gen1**. The dashboard leverages advanced DAX for modeling borrower profiles, credit risk, and loan performance across various dimensions.

---

## 🧾 Dataset Column Descriptions

| Column Name         | Description |
|---------------------|-------------|
| **LoanID**          | Unique identifier for each loan. |
| **Age**             | Borrower's age when the loan was issued. |
| **Income**          | Borrower's annual income. |
| **LoanAmount**      | Approved or requested loan amount. |
| **CreditScore**     | Creditworthiness score (300–850 range). |
| **MonthsEmployed**  | Months employed at current job. |
| **NumCreditLines**  | Total number of active credit lines (e.g., loans, credit cards). |
| **InterestRate**    | Annual percentage rate charged on the loan. |
| **LoanTerm**        | Duration (in months) of loan repayment. |
| **DTIRatio**        | Debt-to-Income ratio indicating financial stress. |
| **Education**       | Highest education level attained. |
| **EmploymentType**  | Employment status (e.g., Full-Time, Part-Time, etc.). |
| **MaritalStatus**   | Marital status of the borrower. |
| **HasMortgage**     | Whether borrower has an existing mortgage. |
| **HasDependents**   | Whether borrower has financial dependents. |
| **LoanPurpose**     | Reason for taking the loan (e.g., Home, Education, Auto). |
| **HasCoSigner**     | Indicates if loan has a co-signer. |
| **Default**         | Indicates if borrower defaulted on the loan. |
| **Loan Date (DD/MM/YYYY)** | Date the loan was issued. |

---

## 🔄 Data Ingestion

- Loaded data using **Power BI Dataflow Gen1** from a **local SQL Server** source.
- Over **250,000 records** were processed and cleaned for use in Power BI.
- Data transformations included binning credit scores, creating age groups, and calculating income brackets.

---

## 🧠 DAX Measures Used

### 📈 Financial & Risk Metrics
- **Loan Amount by Purpose**  
- **Default Rate by Employment Type**  
- **Default Rate by Year**  
- **YOY Loan Amount Change**  
- **YOY Default Loans Change**

### 👥 Demographics-Based Measures
- **Average Loan by Age Group**  
- **Average Income by Employment Type**  
- **Loans by Education Type**  
- **Total Loan by Credit Score Bins & Age Group**

### 🎯 Segmentations
- **Credit Score Bins** (`Very Low`, `Low`, `Medium`, `High`)  
- **Income Bracket** (`Low Income`, `Medium Income`, `High Income`)  
- **Age Groups** (`Teen`, `Adults`, `Middle Age Adults`, `Senior Citizens`)

---

## 📊 Report Pages & Visual Sections

### 📍 Page 1: Loan Default & Overview
- Loan distribution by purpose and average income by employment type
- Default rates across employment categories and yearly trend
- Age-wise analysis of average loan amount

**![Loan Default Overview Page](![Image](https://github.com/user-attachments/assets/dc192f89-9690-4482-92da-c7d770e58fb1))**

---

### 📍 Page 2: Applicant Demographics & Financial Profile
- Median and average loan amounts by credit score and marital status
- Loan segmentation by dependents, mortgage status, and education level

**![Applicant Demographics Page](path/to/image2.png)**

---

### 📍 Page 3: Financial Risk Metrics
- YOY changes in loan disbursal and default behavior
- Income-employment-credit segmentation using Sankey and treemap visuals

**![Financial Risk Metrics Page](path/to/image3.png)**

---

## 🛠 Tools & Technologies

- Power BI Desktop  
- Power BI Dataflow Gen1  
- SQL Server (Local)  
- DAX (Data Analysis Expressions)

---

## 📎 Author

**Karandeep Singh**  
[LinkedIn](https://linkedin.com/in/karandeep-singh-concordia)  
