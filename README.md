![Mostafa Osama — Data Analyst banner with dark purple and cyan aurora accents](./.github/assets/readme-aura-component-0-036f33ab.svg)

# Hi, I'm Mostafa Osama

**Data Analyst | SQL, Power BI, Excel & Python | Building dashboards and turning data into clear business insights.**

Based in Cairo, Egypt. I build end-to-end analytics projects spanning SQL database design, data cleaning and transformation (Power Query & Python), data modeling, and interactive dashboards in Power BI and Excel.

![](./.github/assets/readme-aura-component-1-f663e73f.svg)

## Featured Projects

### 1. [Olist E-Commerce Analytics](https://github.com/MostafaOsama0/Olist-ECommerce-Analytics)

**Stack:** Power BI · DAX · Power Query

Interactive multi-page Power BI report built on the Brazilian Olist public e-commerce dataset, combining bookmark-driven Orders and Customers dashboards with raw data views, interactive slicers, payment-method breakdowns, and regional delivery analysis.

* **Key pattern:** The customer satisfaction analysis highlights an association between longer delivery times and lower customer review scores, alongside a high share of single-purchase buyers across Brazilian states.

![Olist Customers Power BI dashboard showing review score distribution, customer loyalty split, top Brazilian states, and delivery time versus review score chart](https://raw.githubusercontent.com/MostafaOsama0/Olist-ECommerce-Analytics/main/Screenshots/Customers%20Dashboard.png)

***

### 2. [HR Database Management System (SQL)](https://github.com/MostafaOsama0/HR-Database-Management-SQL)

**Stack:** Microsoft SQL Server · T-SQL · Relational Schema Design

Normalized 7-table relational HR database (`Employees`, `Departments`, `JobTitles`, `Tasks`, `EmployeesTitleHistory`, `EmployeesDepartmentHistory`, and `EmployeesTasks`) with a self-referencing manager hierarchy (`ManagerID`), staging data load (`tmp_employees.csv`), and 10 analytical T-SQL reporting queries.

* **Demonstrated capability:** Enforces domain rules directly in the schema via `PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, and `CHECK` constraints (minimum hiring age of 21, hire dates on or after `2010-07-01`, and `0–100` graduation grade bounds) and queries workforce records with multi-table joins, self-joins, `GROUP BY`/`HAVING`, date filters, and `NOT EXISTS` anti-joins.

![SQL Server entity-relationship diagram for the ICTHub_HR database showing seven normalized HR tables and the tmp_employees staging table](https://raw.githubusercontent.com/MostafaOsama0/HR-Database-Management-SQL/main/ICTHub_D1.png)

<details>
<summary>View genuine T-SQL schema constraints &amp; reporting query excerpt (from <code>ICTHUB_HR_FINALPROJECT.sql</code>)</summary>

```sql
-- Domain integrity constraints & self-referencing hierarchy on Employees
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY,
    FirstName NVARCHAR(25) NOT NULL,
    LastName NVARCHAR(25) NOT NULL,
    BirthDate DATE NOT NULL,
    Nationality NVARCHAR(50) NOT NULL,
    HiringDate DATE NOT NULL,
    GraduationGradePercentage DECIMAL(5,2),
    DepartmentID INT FOREIGN KEY REFERENCES Departments(DepartmentID),
    ManagerID INT NULL REFERENCES Employees(EmployeeID),
    CONSTRAINT CHK_HiringDate CHECK (HiringDate >= '2010-07-01'),
    CONSTRAINT EMP_AGE CHECK (HiringDate >= DATEADD(YEAR, 21, BirthDate)),
    CONSTRAINT CHK_GraduationGrade CHECK (GraduationGradePercentage BETWEEN 0.00 AND 100.00)
);

-- Managers leading fewer than two direct reports (self-join + HAVING)
SELECT
    M.EmployeeID AS ManagerID,
    CONCAT(M.FirstName, ' ', M.LastName) AS [Full Name],
    COUNT(E.EmployeeID) AS [#Leadings]
FROM Employees M
JOIN Employees E
    ON M.EmployeeID = E.ManagerID
GROUP BY M.EmployeeID, M.FirstName, M.LastName
HAVING COUNT(E.EmployeeID) < 2;
```

</details>

***

### 3. [UK YouTubers ROI Analysis](https://github.com/MostafaOsama0/UK_Youtubers_ROI_Analysis)

**Stack:** SQL Server (T-SQL) · Power BI · DAX

Two-stage BI workflow combining T-SQL data preparation (`Sql code`) with a two-page Power BI report (`Influencer Profitability Simulator` and `The Deep Dive`) built around interactive What-If parameters for conversion rate, product cost, and campaign cost.

* **Demonstrated capability:** Cleans raw channel names into a structured SQL view (`view_Uk_Youtubers`), runs row-count, schema-column, and duplicate-channel validation checks, and models channel-level scenario estimates with a T-SQL CTE (`ChannelData`) and Power BI What-If slicers.

<details>
<summary>View genuine T-SQL view &amp; data-validation excerpt (from <code>Sql code</code>)</summary>

```sql
CREATE VIEW view_Uk_Youtubers AS
SELECT
    CAST(SUBSTRING(nombre, 1, CHARINDEX('@', NOMBRE) - 1) AS VARCHAR(100)) AS Channel_name,
    [total_subscribers],
    [total_views],
    [total_videos]
FROM youtube_data_from_python;

-- Duplicate channel check
SELECT Channel_name, COUNT(Channel_name)
FROM view_Uk_Youtubers
GROUP BY Channel_name
HAVING COUNT(Channel_name) > 1;
```

</details>

***

<details>
<summary><strong>More Analytics Projects (9 Power BI &amp; Excel Dashboards)</strong></summary>

<br />

| Project | Tools | Summary |
| :--- | :--- | :--- |
| [US Sales Data Analysis](https://github.com/MostafaOsama0/US_Dataset-Project) | Excel | Multi-sheet US sales workbook (`US_Dataset Project.xlsx`) with Home navigation, Pivot Tables, a 2015–2018 Sales Performance Dashboard, and a State Distribution Map tracking sales and profit by region, ship mode, category, sub-category, top products, and discount levels. |
| [Pizza Store Sales Analysis](https://github.com/MostafaOsama0/Pizza-Store) | Power BI, Power Query | Interactive Power BI report (`Pizza Store Power Bi.pbix`) tracking store sales KPIs, order volume, and product/category performance across Home and Sales Performance views. |
| [Coffee Shop Analytics](https://github.com/MostafaOsama0/Coffee-shop-Project) | Power BI, Power Query | Three-page Power BI report (`Coffee shop.pbix`) covering Home overview, product demand analysis, and customer insights. |
| [HR Project](https://github.com/MostafaOsama0/HR-Project) | Power BI, Power Query | Power BI workforce report (`HR Analysis.pbix`) analyzing employee overview metrics, salary distributions, demographics, and attrition trends. |
| [HR Analysis](https://github.com/MostafaOsama0/HR-Analysis) | Power BI, Power Query | Multi-page Power BI HR reporting layout covering Home, Payroll, and Employee views. |
| [Social Media Metrics Dashboard](https://github.com/MostafaOsama0/Social-media-metrics-Project) | Excel | Excel workbook (`Social-Media-Metrics Project.xlsx`) with dataset, Pivot Tables, and KPI dashboard tracking likes, comments, shares, impressions, and follower trends across platforms. |
| [Sales Dataset Analysis](https://github.com/MostafaOsama0/Sales_Dataset-Project) | Excel | Excel sales workbook (`Sales_Dataset Project.xlsx`) combining transaction data, Pivot Tables, and a dashboard tracking revenue, orders, regions, and customer segments. |
| [Vrinda Store Analysis](https://github.com/MostafaOsama0/Vrinda-store-Analysis) | Excel | Excel sales and demographics dashboard (`Vrinda Store Project.xlsx`) tracking monthly orders, customer age/gender segments, order status, states, and sales channels. |
| [Bike Store Project](https://github.com/MostafaOsama0/Bike-Store-Project) | Excel | Excel workbook (`Bike store.xlsx`) and dashboard analyzing bike store sales, product performance, and customer demographics. |

</details>

![](./.github/assets/readme-aura-component-2-d4d96541.svg)

## Skills & Tools

| Category | Stack & Capabilities |
| :--- | :--- |
| **Languages & Querying** | SQL (SQL Server / T-SQL), Python (Pandas, NumPy, Matplotlib) |
| **BI & Spreadsheets** | Power BI (DAX, Power Query, Bookmark Navigation), Microsoft Excel (Pivot Tables, Formulas, Conditional Formatting, Charts) |
| **Analytics & Methods** | Data Modeling, ETL & Data Cleaning, Statistics, KPI Design, Data Storytelling, AI Automation |
| **Analytics & Dev Workspace** | Jupyter Notebook, VS Code, SQL Server, Power BI Desktop, Microsoft Excel |
| **Version Control** | Git, GitHub |

## Education

**Bachelor of Computer Science**\
Benha National University, Obour, Qalyubia, Egypt\
*Expected Graduation: 2027*

## Contact

* **LinkedIn:** [linkedin.com/in/mostafaosama0](https://www.linkedin.com/in/mostafaosama0/)
* **Email:** <mostafaosama7213@gmail.com>
