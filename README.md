
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

### 📈 Key Metrics & Measures

- `Loan Amount by Purpose`: Aggregates loan volume by use-case categories.
- `Average Income by Employment Type`: Compares average income across employment groups.
- `Default Rate by Employment Type` and `Default Rate by Year`: Tracks loan performance by employment status and over time.
- `YOY Loan Amount Change` and `YOY Default Loans Change`: Measures year-over-year performance trends.
- `Median by Credit Score Bins`: Identifies central tendency across borrower risk profiles.
- `Average Loan by Age Group`: Shows age-wise borrowing capacity.
- `Total Loan (Middle Age Adults)` and `Total Loan (Credit Bins)`: Analyze loan volume among risk segments.
- `Income Bracket`: Segments users by income level (Low, Medium, High).
- `Credit Score Bins`: Categorizes borrowers into Very Low, Low, Medium, and High tiers.

---

## 📊 Report Pages & Analysis

### 📍 Page 1: Loan Default & Overview

**DAX Highlights**:  
- `Loan Amount by Purpose`, `Average Income by Employment Type`, `Default Rate by Employment Type`, `Average Loan by Age Group`, `Default Rate by Year`

**Insights**:
- Home loans dominate total disbursement, with full-time employed individuals earning the most.
- Unemployed borrowers show the highest default rates.
- Adults aged 20–39 tend to borrow more, and default rates fluctuate between 11.5%–11.75% over the years.

![Image](https://github.com/user-attachments/assets/dc192f89-9690-4482-92da-c7d770e58fb1)

---

### 📍 Page 2: Applicant Demographics & Financial Profile

**DAX Highlights**:  
- `Median by Credit Score Bins`, `Average Loan Amt (High Credit Score)`, `Total Loan (Credit Bins)`, `Total Loan (Middle Age Adults)`, `Loans by Education Type`

**Insights**:
- Borrowers with high credit scores receive the highest loan amounts, with consistency across marital status and age.
- Adults and middle-aged applicants hold the bulk of total disbursed amounts.
- Bachelor’s degree holders lead in loan frequency, suggesting education may play a role in eligibility.

![Image](https://github.com/user-attachments/assets/38d601ac-e96d-44b0-82f4-1ac5ab9d97b7)

---

### 📍 Page 3: Financial Risk Metrics

**DAX Highlights**:  
- `YOY Loan Amount Change`, `YOY Default Loans Change`, `Income Bracket`, `EmploymentType`

**Insights**:
- YOY analysis reveals peaks and dips in both loan issuance and default rates (notably in 2015 and 2017).
- Sankey visuals reveal high-income individuals take the majority of loans across employment types.
- Risk stratification through income and employment segmentation helps identify high-value and low-risk segments.

![Image](https://github.com/user-attachments/assets/207f5aee-8f88-4832-b812-033486397c31)

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
[GitHub](https://github.com/Devilo24)
