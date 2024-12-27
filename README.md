## Zomato Power BI Project

### 1. Project Objective
**Purpose**: Analyze sales performance, user performance, and city-wise performance for Zomato, an online food delivery app.  
**Audience**: Management team  
**Key Deliverables**:  
- Yearly sales values segmented by city  
- Comparison of vegetarian and non-vegetarian sales  
- User gain and loss metrics  
- User demographics by age group and corresponding sales data  
- Customer ratings and user distribution by city  

### 2. Data Sources
**Data Origin**: Excel files  
**Data Volume**:  
- **Sheet 1 (Food)**: 371,561 rows, 3 columns  
- **Sheet 2 (Menu)**: 1,048,575 rows, 6 columns  
- **Sheet 3 (Order)**: 1,048,576 rows, 5 columns  
- **Sheet 4 (Restaurants)**: 148,541 rows, 9 columns  
- **Sheet 5 (Order Type)**: 150,282 rows, 2 columns  
- **Sheet 6 (Users)**: 100,001 rows, 6 columns  

**Data Model**: Star schema for efficient data organization  

### 3. Key Metrics and KPIs
- Total sales by year and city  
- Sales split between vegetarian and non-vegetarian items  
- User retention rates (gains and losses)  
- Sales metrics categorized by user age groups  
- Average ratings per city  

### 4. Visualizations and Reports
**Dashboards**:  
- Cards, Donut charts, Clustered bar charts, Clustered column charts, Line charts, Matrix cards

**Filters and Interactions**:  
- Slicers and interactive buttons for enhanced user experience
  
**Page Layout**:
- **Page 1**: Index
![Zomato_index](https://github.com/user-attachments/assets/98042084-ab8f-405e-9b42-0555a5cc9e1b)

- **Page 2**: Overview
![Zomato_overview](https://github.com/user-attachments/assets/a9d1f805-179f-4f03-944e-e9e1d14fcbe5)

- **Page 3**: User Performance
![Zomato_user](https://github.com/user-attachments/assets/8e13b6b9-fc11-4d85-9245-3fe0c162a5dd)

- **Page 4**: City Dashboard
![Zomato_city](https://github.com/user-attachments/assets/c8486e0e-0a93-4998-a212-7be8e6bbf412)


### 5. Data Analysis
**Transformations**:  
- Replacing values, merging queries, renaming columns, expanding and unpivoting tables

**Calculated Fields**:  
- DAX functions: `SUM`, `FORMAT`, `COUNT`, `RANKX`, `SELECTEDVALUE`, `DISTINCTCOUNT`, `SUMMARIZE`  

### 6. Challenges and Solutions

- **Challenge 1**: Difficulty in identifying gained and lost customers.<br>
  **Solution**: Implemented custom DAX formulas to track customer gain and loss by comparing users' order histories across time periods.

- **Challenge 2**: Performance optimization for large datasets (e.g., over 1 million rows).<br>
  **Solution**: Used data reduction techniques like aggregations and efficient query modeling to improve performance.

- **Challenge 3**: Handling incomplete or inconsistent data from Excel files.<br>
  **Solution**: Applied data cleaning steps in Power Query, including removing duplicates, filling missing values, and ensuring data quality.



