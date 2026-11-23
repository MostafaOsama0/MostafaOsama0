<!-- aura-alt: Mostafa Osama — Data Analyst banner with dark purple and cyan aurora accents -->
```aura width=800 height=225
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#07070d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.28)' }}>
  <style>{`
    @keyframes h-orb-1 { 0%, 100% { transform: translate(0, 0); opacity: 0.6; } 50% { transform: translate(32px, -18px); opacity: 0.9; } }
    @keyframes h-orb-2 { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(-26px, 16px); opacity: 0.82; } }
    @keyframes h-ring { 0%, 100% { opacity: 0.06; } 50% { opacity: 0.17; } }
    @keyframes h-wave { 0% { stroke-dashoffset: 900; } 100% { stroke-dashoffset: 0; } }
    @keyframes h-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    #h-o1 { animation: h-orb-1 9s ease-in-out infinite; }
    #h-o2 { animation: h-orb-2 11s ease-in-out infinite 0.6s; }
    #h-o3 { animation: h-orb-1 10s ease-in-out infinite 1.5s; }
    #h-r1 { animation: h-ring 7.5s ease-in-out infinite; }
    #h-r2 { animation: h-ring 8.5s ease-in-out infinite 2s; }
    #h-orbit { transform-origin: 400px 112px; animation: h-spin 20s linear infinite; }
    #h-spark { stroke-dasharray: 900; animation: h-wave 5.5s linear infinite; }
  `}</style>

  <svg width="800" height="225" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hg-violet" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.6)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="hg-cyan" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,211,238,0.5)" />
        <stop offset="70%" stopColor="rgba(34,211,238,0)" />
      </radialGradient>
      <radialGradient id="hg-indigo" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(79,70,229,0.48)" />
        <stop offset="70%" stopColor="rgba(79,70,229,0)" />
      </radialGradient>
      <linearGradient id="hg-line" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(139,92,246,0)" />
        <stop offset="35%" stopColor="rgba(139,92,246,0.65)" />
        <stop offset="65%" stopColor="rgba(34,211,238,0.75)" />
        <stop offset="100%" stopColor="rgba(34,211,238,0)" />
      </linearGradient>
    </defs>

    <ellipse id="h-o1" cx="145" cy="195" rx="240" ry="135" fill="url(#hg-violet)" />
    <ellipse id="h-o2" cx="675" cy="40" rx="230" ry="135" fill="url(#hg-cyan)" />
    <ellipse id="h-o3" cx="605" cy="205" rx="195" ry="120" fill="url(#hg-indigo)" />

    <circle id="h-r1" cx="400" cy="112" r="68" fill="none" stroke="rgba(196,181,253,0.9)" strokeWidth="0.7" />
    <circle id="h-r2" cx="400" cy="112" r="118" fill="none" stroke="rgba(165,243,252,0.85)" strokeWidth="0.7" />
    <g id="h-orbit">
      <circle cx="400" cy="44" r="2.8" fill="#22d3ee" />
    </g>

    <path id="h-spark" d="M 0 198 Q 95 190, 165 195 T 320 183 T 485 191 T 640 179 T 800 189" fill="none" stroke="url(#hg-line)" strokeWidth="1.5" />
  </svg>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
    <span style={{ fontSize: 48, fontWeight: 700, color: '#ffffff', letterSpacing: -1.4, lineHeight: 1.05 }}>Mostafa Osama</span>
    <span style={{ fontSize: 15, fontWeight: 600, color: '#67e8f9', marginTop: 12, letterSpacing: 5, textTransform: 'uppercase' }}>Data Analyst</span>
    <div style={{ display: 'flex', gap: 10, marginTop: 22 }}>
      <span style={{ padding: '5px 15px', background: 'rgba(17,15,31,0.72)', color: '#67e8f9', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(34,211,238,0.3)' }}>SQL</span>
      <span style={{ padding: '5px 15px', background: 'rgba(17,15,31,0.72)', color: '#c4b5fd', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(139,92,246,0.32)' }}>Power BI</span>
      <span style={{ padding: '5px 15px', background: 'rgba(17,15,31,0.72)', color: '#86efac', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(74,222,128,0.28)' }}>Excel</span>
      <span style={{ padding: '5px 15px', background: 'rgba(17,15,31,0.72)', color: '#a5b4fc', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(129,140,248,0.3)' }}>Python</span>
    </div>
  </div>
</div>
```

# Hi, I'm Mostafa Osama

**Data Analyst | SQL, Power BI, Excel & Python | Building dashboards and turning data into clear business insights.**

Based in Cairo, Egypt. I build end-to-end analytics projects spanning SQL database design, data cleaning and transformation (Power Query & Python), data modeling, and interactive dashboards in Power BI and Excel.

**Connect:** [LinkedIn](https://www.linkedin.com/in/mostafaosama0/) · [Email](mailto:mostafaosama7213@gmail.com)

<!-- aura-alt:  -->
```aura width=800 height=14
<div style={{ position: 'relative', display: 'flex', width: '100%', height: '100%', background: 'transparent', overflow: 'hidden' }}>
  <style>{`
    @keyframes div1-sweep { 0% { transform: translateX(-220px); } 100% { transform: translateX(860px); } }
    #div1-beam { animation: div1-sweep 5s linear infinite; }
  `}</style>
  <svg width="800" height="14" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="div1-base" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(139,92,246,0)" />
        <stop offset="25%" stopColor="rgba(139,92,246,0.45)" />
        <stop offset="75%" stopColor="rgba(34,211,238,0.45)" />
        <stop offset="100%" stopColor="rgba(34,211,238,0)" />
      </linearGradient>
      <linearGradient id="div1-glow" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(34,211,238,0)" />
        <stop offset="50%" stopColor="rgba(103,232,249,0.9)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </linearGradient>
    </defs>
    <rect x="0" y="6" width="800" height="2" rx="1" fill="url(#div1-base)" />
    <rect id="div1-beam" x="0" y="5" width="180" height="4" rx="2" fill="url(#div1-glow)" />
  </svg>
</div>
```

## Featured Projects

### 1. [Olist E-Commerce Analytics](https://github.com/MostafaOsama0/Olist-ECommerce-Analytics)
**Stack:** Power BI · DAX · Power Query

Interactive multi-page Power BI report built on the Brazilian Olist public e-commerce dataset, combining bookmark-driven Orders and Customers dashboards with raw data views, interactive slicers, payment-method breakdowns, and regional delivery analysis.

- **Key pattern:** The customer satisfaction analysis highlights an association between longer delivery times and lower customer review scores, alongside a high share of single-purchase buyers across Brazilian states.

![Olist Customers Power BI dashboard showing review score distribution, customer loyalty split, top Brazilian states, and delivery time versus review score chart](https://raw.githubusercontent.com/MostafaOsama0/Olist-ECommerce-Analytics/main/Screenshots/Customers%20Dashboard.png)

---

### 2. [HR Database Management System (SQL)](https://github.com/MostafaOsama0/HR-Database-Management-SQL)
**Stack:** Microsoft SQL Server · T-SQL · Relational Schema Design

Normalized 7-table relational HR database (`Employees`, `Departments`, `JobTitles`, `Tasks`, `EmployeesTitleHistory`, `EmployeesDepartmentHistory`, and `EmployeesTasks`) with a self-referencing manager hierarchy (`ManagerID`), staging data load (`tmp_employees.csv`), and 10 analytical T-SQL reporting queries.

- **Demonstrated capability:** Enforces domain rules directly in the schema via `PRIMARY KEY`, `FOREIGN KEY`, `UNIQUE`, and `CHECK` constraints (minimum hiring age of 21, hire dates on or after `2010-07-01`, and `0–100` graduation grade bounds) and queries workforce records with multi-table joins, self-joins, `GROUP BY`/`HAVING`, date filters, and `NOT EXISTS` anti-joins.

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

---

### 3. [UK YouTubers ROI Analysis](https://github.com/MostafaOsama0/UK_Youtubers_ROI_Analysis)
**Stack:** SQL Server (T-SQL) · Power BI · DAX

Two-stage BI workflow combining T-SQL data preparation (`Sql code`) with a two-page Power BI report (`Influencer Profitability Simulator` and `The Deep Dive`) built around interactive What-If parameters for conversion rate, product cost, and campaign cost.

- **Demonstrated capability:** Cleans raw channel names into a structured SQL view (`view_Uk_Youtubers`), runs row-count, schema-column, and duplicate-channel validation checks, and models channel-level scenario estimates with a T-SQL CTE (`ChannelData`) and Power BI What-If slicers.

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

---

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

<!-- aura-alt:  -->
```aura width=800 height=14
<div style={{ position: 'relative', display: 'flex', width: '100%', height: '100%', background: 'transparent', overflow: 'hidden' }}>
  <style>{`
    @keyframes div2-sweep { 0% { transform: translateX(860px); } 100% { transform: translateX(-220px); } }
    #div2-beam { animation: div2-sweep 5.5s linear infinite; }
  `}</style>
  <svg width="800" height="14" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="div2-base" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(34,211,238,0)" />
        <stop offset="25%" stopColor="rgba(34,211,238,0.45)" />
        <stop offset="75%" stopColor="rgba(139,92,246,0.45)" />
        <stop offset="100%" stopColor="rgba(139,92,246,0)" />
      </linearGradient>
      <linearGradient id="div2-glow" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(139,92,246,0)" />
        <stop offset="50%" stopColor="rgba(196,181,253,0.9)" />
        <stop offset="100%" stopColor="rgba(34,211,238,0)" />
      </linearGradient>
    </defs>
    <rect x="0" y="6" width="800" height="2" rx="1" fill="url(#div2-base)" />
    <rect id="div2-beam" x="0" y="5" width="180" height="4" rx="2" fill="url(#div2-glow)" />
  </svg>
</div>
```

## Skills & Tools

| Category | Stack & Capabilities |
| :--- | :--- |
| **Languages & Querying** | SQL (SQL Server / T-SQL), Python (Pandas, NumPy, Matplotlib) |
| **BI & Spreadsheets** | Power BI (DAX, Power Query, Bookmark Navigation), Microsoft Excel (Pivot Tables, Formulas, Conditional Formatting, Charts) |
| **Analytics & Methods** | Data Modeling, ETL & Data Cleaning, Statistics, KPI Design, Data Storytelling, AI Automation |
| **Analytics & Dev Workspace** | Jupyter Notebook, VS Code, SQL Server, Power BI Desktop, Microsoft Excel |
| **Version Control** | Git, GitHub |

## Education

**Bachelor of Computer Science**  
Benha National University, Obour, Qalyubia, Egypt  
*Expected Graduation: 2027*

## Contact

- **LinkedIn:** [linkedin.com/in/mostafaosama0](https://www.linkedin.com/in/mostafaosama0/)
- **Email:** [mostafaosama7213@gmail.com](mailto:mostafaosama7213@gmail.com)
