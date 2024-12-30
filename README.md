# **Hospital Patient Records Data Pipeline**

## **Overview**
This Python script demonstrates a robust **data pipeline** I developed as part of a healthcare analytics project. It automates the process of **loading**, **cleaning**, **normalizing**, and **uploading** data from CSV files into a **MySQL database**, transforming raw healthcare data into structured, ready-to-analyze tables.

The pipeline was designed to emulate real-world data workflows, ensuring scalability, automation, and maintainability. By consulting and even **correcting ChatGPT**, I showcased my strong understanding of Python fundamentals and ability to refine solutions through **effective prompt engineering**.

---

## **Key Features**
- **Automated Data Loading**:
  - Efficiently reads and processes multiple CSV files (encounters, patients, procedures, etc.).
  - Ensures data integrity by explicitly defining column data types, such as treating ZIP codes as strings to preserve formatting.
  
- **Data Cleaning**:
  - Handles edge cases, such as blank or malformed values in critical columns.
  - Applies string transformations (e.g., removing invalid characters) and ensures correct date formatting (`YYYY-MM-DD` or `YYYY-MM-DD HH:MM:SS`).

- **Data Normalization**:
  - Creates unique identifiers for primary keys and maps foreign keys for relational consistency.
  - Drops unnecessary or redundant columns, ensuring clean and structured data.

- **Database Integration**:
  - Automates the upload of normalized tables into a MySQL database using SQLAlchemy.
  - Supports dynamic updates while preserving relational constraints like foreign keys.

---

## **Skills Demonstrated**
### **Python Comprehension**:
- Leveraged advanced features like:
  - **Pandas** for data manipulation.
  - **Lambda functions** for custom transformations.
  - **String methods** to handle formatting challenges.
- Wrote modular, reusable functions for scalability.

### **Effective Prompt Engineering**:
- Consulted ChatGPT to address complex challenges, including:
  - Preserving leading zeros in ZIP codes.
  - Handling blank values dynamically.
  - Optimizing data cleaning steps for performance and readability.
- **Corrected ChatGPT** when necessary:
  - Identified and rectified inefficiencies in suggested solutions.
  - Provided precise and iterative prompts to achieve a tailored, efficient Python script.

### **Relational Database Skills**:
- Designed and normalized relational tables in MySQL.
- Implemented strategies to handle foreign key constraints and ensure data consistency.
- Utilized MySQL data types (e.g., `VARCHAR`, `DATETIME`) effectively.
