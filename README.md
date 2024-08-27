## **Process**

### **1. Data Understanding and Requirements Gathering**
- Gather business requirements and identify key metrics and data sources.

### **2. Data Modeling**
- Design the star schema with fact and dimension tables.

### **3. Data Extraction, Transformation, and Loading (ETL)**
- Extract data from source systems.
- Transform data to fit the star schema and ensure data quality.
- Load the transformed data into the fact and dimension tables.

### **4. Data Validation and Quality Assurance**
- Implement validation rules and perform data quality checks to ensure integrity and accuracy.

### **5. Handling Row Dropping**
- Address rows with invalid data (e.g., `SalesAmount` ≤ 0) by either correcting or dropping them as per business rules.

### **6. Reporting and Analytics**
- Develop reports and dashboards that utilize the star schema for business insights.
