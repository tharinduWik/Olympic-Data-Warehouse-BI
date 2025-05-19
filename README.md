![Screenshot 2025-05-20 002314](https://github.com/user-attachments/assets/65837e2d-d3c6-4048-a344-a12228f31969)# Olympic Data Warehouse and Business Intelligence Project

![Power BI Dashboard](Screenshots/BiHomepage.png)

## Overview
This project, developed as part of the Data Warehouse & Business Intelligence course (IT3021) at Sri Lanka Institute of Information Technology, demonstrates the design and implementation of a data warehouse and BI solution using Olympic Games data. The project includes a snowflake schema-based data warehouse, an SSAS cube for multidimensional analysis, OLAP operations in Excel, and interactive Power BI reports to uncover insights into Olympic medal achievements.

## Project Components
1. **Data Warehouse (Olympic_DW)**:
   - Designed a snowflake schema in SQL Server with one fact table (`MedalsList`) and dimension tables (`Athlete`, `Country`, `Event`, `Year`, `MedalType`, `Discipline`).
   - Fact table measures: `MedalCount`, `MedalID`.
   - Normalized dimension tables to reduce redundancy and optimize query performance.
   - Tools: SQL Server, SQL Server Management Studio (SSMS).

2. **SSAS Cube**:
   - Built a cube (`Cube_Olympic_DW`) using SQL Server Analysis Services (SSAS) and SQL Server Data Tools (SSDT).
   - Measures: Sum of `MedalCount` (TotalMedals).
   - Dimensions: Athlete, Country, Event, Year, MedalType, Discipline.
   - Hierarchy: Country to Continent for aggregated analysis.

3. **OLAP Operations**:
   - Performed Slice, Dice, Roll-up, Drill-down, and Pivot operations using Excel pivot tables and charts.
   - Connected Excel to the SSAS cube for dynamic data exploration.

4. **Power BI Reports**:
   - Created four interactive reports hosted on Power BI Service:
     - Matrix visual with Country, Athlete, and Year.
     - Slicers with cascading filters for Country and Athlete.
     - Drill-down chart with DateHierarchy (Year > Quarter > Month).
     - Drill-through report for country-specific athlete details.
   - Link: [Power BI Report](https://app.powerbi.com/links/aGQDrv8xE?ctid=44e3cf94-19c9-4e32-96c3-14f5bf01391a&pbi_source=linkShare)

## Repository Structure
- `scripts/`: SQL scripts for data warehouse creation and ETL processes.
- `docs/`: Project documentation (e.g., IT22562456.pdf).
- `screenshots/`: Images of SSAS cube, Excel pivot tables, and Power BI dashboards.
- `requirements.txt`: List of dependencies (e.g., SQL Server, Power BI Desktop).

## Setup Instructions
1. **Prerequisites**:
   - SQL Server (16.0 or later), SSMS, SSDT, SSAS, Power BI Desktop.
2. **Steps**:
   - Clone this repository: `git clone https://github.com/yourusername/Olympic-Data-Warehouse-BI.git`.
   - Import SQL scripts into SQL Server to create the Olympic_DW database.
   - Deploy the SSAS cube using SSDT.
   - Connect Excel or Power BI to the SSAS cube for analysis.
   - View Power BI reports via the provided link.

## Technologies Used
- **Database**: SQL Server, SSAS
- **Tools**: SSDT, SSMS, Excel, Power BI Desktop, Power BI Service
- **Concepts**: Data Warehousing, Snowflake Schema, OLAP, Data Visualization

## Screenshots
![SSAS Cube](screenshots/ssas_cube.png)
![Excel Pivot Table](screenshots/excel_pivot.png)

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
H.M.T.W Dilshan | [LinkedIn](https://www.linkedin.com/in/yourprofile) | [Email](mailto:your.email@example.com)
