# Power BI – Transforming Multiple Data Sources

## Project Overview
This project demonstrates how to clean, transform, and merge multiple data sources in Power BI using Power Query. The project covers ETL (Extract, Transform, Load) techniques, anomaly detection, and data profiling.

## Steps Performed in the Project
1. **Set up the Power BI Project**: 
   - Created a new Power BI project called **"Exercise – Transforming Multiple Data Sources"**.
   - Imported the provided data files: `Order2022.xlsx`, `Order2023.xlsx`, and `OrderDetails.xlsx`.

2. **Data Transformation in OrderDetails**: 
   - Opened the **OrderDetails** table and kept only the relevant columns: `SalesOrderID`, `ProductID`, `OrderQty`, and `UnitPrice`.
   - Removed any unnecessary columns to focus on key data.

3. **Data Profiling**:
   - Applied **Column Distribution**, **Column Quality**, and **Column Profile** tools in Power Query to analyze the data.
   - Identified and noted the number of distinct and unique values in the `UnitPrice` column.
   - Detected potential anomalies by profiling the `UnitPrice` column and finding outliers.

4. **Anomaly Detection**:
   - Found three rows with outliers in the `UnitPrice` column, suspected to be data entry mistakes.
   - Filtered and removed these rows to avoid incorrect calculations and ensure accurate analysis.

5. **Appending Data**:
   - Appended the 2022 and 2023 sales data (`Order2022` and `Order2023`) into a new master table called **Orders**.
   - Verified the appending process by checking the column names, row counts, and data consistency.

6. **Merging Data**:
   - Merged the **Orders** table with the **OrderDetails** table based on the common column `SalesOrderID`.
   - Chose the **Inner Join** method to select matching records.
   - Expanded the merged table to include the `OrderDate` column from the **Orders** table.
   - Renamed the expanded column to `OrderDate` for clarity.

## Skills Used
- **Power Query** for data transformation and cleaning.
- **Data Transformation** 
- **Data Profiling** and **Anomaly Detection** using Power BI tools.
- **Merging** and **Appending** data from multiple sources.

## Files Included
- `Order2022.xlsx`: Sales data for 2022.
- `Order2023.xlsx`: Sales data for 2023.
- `OrderDetails.xlsx`: Detailed sales data.
- `Exercise – Transforming Multiple Data Sources.pbix`: Power BI report file containing the transformations and analysis.

## How to Use
1. Download the data files from this repository.
2. Open the `.pbix` file in Power BI Desktop.
3. Review the transformations and data anomalies detection process.
4. Explore the data visualization and analysis results.

## Conclusion
This project provides hands-on experience in transforming multiple data sources, cleaning data, merging tables, and identifying and removing data anomalies in Power BI.

