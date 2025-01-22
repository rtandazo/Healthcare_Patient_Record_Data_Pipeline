# **Healthcare Patient Record Data Pipeline with Python and MySQL**

---

## **Overview**

This project showcases an end-to-end data pipeline I developed to process, analyze, and visualize healthcare data. Using Python for data cleaning and staging, and MySQL for advanced querying and reporting, I transformed raw healthcare data into meaningful insights.

The pipeline simulates real-world workflows by dynamically integrating production tables with Power Query (Excel) to create a dynamic dashboard. This dashboard automatically updates with new data, offering actionable insights into healthcare operations, financial performance, and patient outcomes.

This analysis examines a hospital's alarming 45.11% readmission rate—three times the national average—driven largely by chronic conditions like CHF, cancer, and HLD, which account for 86% of readmissions. With $63M in uncovered costs, 62% of which stem from uninsured care in ambulatory and urgent care settings, the findings highlight critical gaps in preventive care and chronic disease management. The dashboard provides actionable insights to address these challenges and reduce financial strain.

---

## **Key Features**

### **Python Pipeline**
- **Automated Data Cleaning**:
  - Loaded raw data from multiple CSV files and addressed common quality issues:
    - Preserved leading zeros in ZIP codes and managed blank values dynamically
    - Standardized date formats (`YYYY-MM-DD`, `YYYY-MM-DD HH:MM:SS`)
    - Cleaned name fields by removing invalid characters
  - Used dynamic mapping to normalize primary and foreign keys for relational consistency

- **Dynamic Staging Tables**:
  - Automated the upload of normalized staging tables into MySQL for efficient analysis
  - Maintained relational integrity by dropping redundant columns post-normalization

### **MySQL Queries**
- **Production Views**:
  - Created reusable production views for operational and financial insights, including:
    - **Average Length of Stay (LOS)**: Emergency, urgent care, and inpatient encounters
    - **Readmission Rates**: Inpatient readmissions with CMS-compliant definitions
    - **Spending Insights**: Medicare Spending Per Beneficiary (MSPB) ratios and total cost of care for non-Medicare patients
    - **Non-Covered Claims**: Breakdown of encounters and costs with no payer coverage

- **Advanced Analytical Queries**:
  - Developed complex SQL scripts incorporating:
    - **Window functions** for rankings, totals, and percentages
    - **Common Table Expressions (CTEs)** to modularize and simplify intricate queries
    - **CASE statements** for conditional logic and flagging key trends

### **Dynamic Dashboard**
[Hospital Patient Records Dashboard](https://1drv.ms/x/c/70cd84e1433785ef/EUt9L2Lk1XFAt9IdHCCzQaUBkeq9eiqMu2Fat3iB4FjXbA?e=EiqkZF) 
- Integrated MySQL production views with **Power Query (Excel)**:
  - Built a dynamic dashboard to visualize KPIs such as:
    - Average LOS by encounter type
    - Hospital spending metrics per medical episode
    - Top medical reasons for readmissions
    - Breakdown of non-covered claims and costs
  - Designed for seamless updates, enabling real-time insights with every data refresh

---

## **Skills Demonstrated**

### **Python Skills**
- **Data Cleaning and Transformation**:
  - Utilized **Pandas** for efficient data manipulation and cleanup
  - Designed reusable, modular functions to handle complex cleaning tasks dynamically

- **Automation and Scalability**:
  - Automated data normalization by dynamically mapping primary and foreign keys
  - Optimized data pipelines for scalability to handle growing datasets

- **Database Integration**:
  - Connected Python to MySQL using **SQLAlchemy**, ensuring efficient and error-free data uploads

### **MySQL Skills**
- **Advanced SQL Techniques**:
  - Leveraged **window functions** (e.g., `SUM() OVER()`, `ROW_NUMBER()`) for aggregate and ranking calculations
  - Created **CTEs (Common Table Expressions)** to break down complex logic into digestible steps
  - Used **CASE statements** for dynamic flagging and filtering

- **Relational Database Design**:
  - Designed an **Enhanced Entity-Relationship (EER) Diagram** to ensure relational integrity
  - Defined primary and foreign key constraints to optimize table relationships

- **Production-Ready Queries**:
  - Built production views to streamline insights into patient outcomes, financial performance, and operational efficiency

### **Effective Prompt Engineering**
- Collaborated with **ChatGPT** to address complex challenges and refine the project:
  - **Corrected outputs** and ensured adherence to best practices, showcasing a strong grasp of Python and SQL fundamentals
  - Used precise, iterative prompts to tailor solutions, enhancing both script efficiency and functionality
  - Demonstrated the ability to balance tool-assisted problem-solving with independent critical thinking

### **Business Intelligence Integration**
[Hospital Patient Records Dashboard](https://1drv.ms/x/c/70cd84e1433785ef/EUt9L2Lk1XFAt9IdHCCzQaUBkeq9eiqMu2Fat3iB4FjXbA?e=EiqkZF)
- **Dynamic Dashboarding**:
  - Integrated MySQL views with Power Query to create a live dashboard for monitoring KPIs
  - Enabled decision-making with real-time data visualization
