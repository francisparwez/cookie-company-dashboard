# 🍪 Cookie Company Interactive Dashboard

An interactive **Microsoft Excel dashboard** designed to analyze and visualize Cookie Company sales performance across products, countries, and time periods.

The project demonstrates practical **data cleaning, data-quality validation, exploratory analysis, KPI development, PivotTables, interactive filtering, and dashboard design** using Excel.

---

## 📊 Project Overview

This project analyzes Cookie Company sales data containing information about:

- 🌍 Country
- 🍪 Product
- 📦 Units Sold
- 💰 Revenue
- 💵 Cost
- 📈 Profit
- 📅 Date

The dataset contains sales records across multiple countries and product categories, allowing the dashboard to provide insights into **sales volume, revenue, cost, profitability, product performance, country performance, and monthly trends**.

The project was developed as an **Excel-based data analytics portfolio project**, with an emphasis on transforming raw business data into an interactive and decision-supporting dashboard.

---

## 🎯 Project Objectives

The primary objectives of this project are to:

1. Analyze overall sales performance.
2. Track Revenue, Cost, Profit, and Units Sold.
3. Compare performance across countries.
4. Analyze product-level sales performance.
5. Identify monthly sales and profitability trends.
6. Build interactive visualizations using Excel.
7. Apply data-quality checks before analysis.
8. Demonstrate professional Excel analytics and dashboard development practices.

---

## 🗂️ Dataset

The Excel workbook contains two worksheets:

| Worksheet  | Records | Description                                                   |
| ---------- | ------: | ------------------------------------------------------------- |
| `Data`     |     700 | Primary sales dataset                                         |
| `New Data` |     525 | Additional dataset containing records overlapping with `Data` |

### Dataset Columns

| Column       | Description                              |
| ------------ | ---------------------------------------- |
| `Country`    | Country associated with the sales record |
| `Product`    | Cookie product sold                      |
| `Units Sold` | Number of units sold                     |
| `Revenue`    | Revenue generated from the sale          |
| `Cost`       | Cost associated with the sale            |
| `Profit`     | Profit generated from the sale           |
| `Date`       | Date of the sales record                 |

---

## 🔎 Data Quality Audit

Before building the dashboard, the dataset was reviewed for common data-quality issues.

### Confirmed Findings

| Check                   | Result                  | Status |
| ----------------------- | ----------------------- | ------ |
| Missing values          | None identified         | ✅     |
| Internal duplicate rows | None identified         | ✅     |
| Negative Units Sold     | None identified         | ✅     |
| Negative Revenue        | None identified         | ✅     |
| Negative Cost           | None identified         | ✅     |
| Negative Profit         | None identified         | ✅     |
| Zero Units Sold         | None identified         | ✅     |
| Zero Revenue            | None identified         | ✅     |
| Zero Cost               | None identified         | ✅     |
| Zero Profit             | None identified         | ✅     |
| Invalid country values  | None identified         | ✅     |
| Invalid product values  | None identified         | ✅     |
| Date formatting         | Valid                   | ✅     |
| Profit calculation      | Consistent              | ✅     |
| Cross-sheet duplication | 525 overlapping records | ⚠️     |

### Important Data-Quality Finding

The `New Data` worksheet contains **525 records that exactly match records already present in the `Data` worksheet**.

Therefore, simply appending both worksheets would result in duplicate records and could inflate:

- Revenue
- Cost
- Profit
- Units Sold
- Record counts

The duplicate records were therefore treated as a **data-quality consideration rather than blindly combining both worksheets**.

> **Important:** The repeated `Country + Product + Date` combinations within the dataset were not automatically classified as duplicates because multiple legitimate sales records may exist for the same country, product, and date.

---

## 📈 Key Analytical Areas

The dashboard focuses on several areas of business performance.

### KPI Analysis

Key performance indicators include:

- **Total Revenue**
- **Total Cost**
- **Total Profit**
- **Total Units Sold**
- **Profit Margin**

### Product Analysis

The dashboard enables analysis of:

- Product sales volume
- Product revenue
- Product profitability
- Product contribution to overall performance

### Country Analysis

Performance can be compared across:

- India
- United Kingdom
- Philippines
- Malaysia
- United States

### Time Analysis

The dashboard supports analysis of sales performance over time, including:

- Monthly trends
- Revenue trends
- Profit trends
- Units sold trends

---

## 📊 Dashboard Features

The interactive dashboard uses Excel's analytical and visualization capabilities, including:

- PivotTables
- PivotCharts
- Interactive slicers
- KPI cards
- Bar/column charts
- Trend analysis
- Product comparisons
- Country comparisons
- Interactive filtering

The objective is to allow users to explore the dataset rather than relying solely on static reports.

---

## 🧮 Business Metrics

### Revenue

Revenue represents the total sales value generated.

```text
Revenue = Units Sold × Product Unit Price
```

The dataset uses **product-specific pricing**, rather than a single price across all products.

### Profit

```text
Profit = Revenue - Cost
```

The dataset was validated against this relationship, with the recorded Profit values remaining consistent with Revenue minus Cost.

### Profit Margin

```text
Profit Margin = (Profit / Revenue) × 100
```

Profit Margin provides an additional measure of profitability beyond absolute profit.

---

## 🛠️ Tools & Technologies

- **Microsoft Excel**
- PivotTables
- PivotCharts
- Excel Slicers
- Excel formulas
- Data cleaning
- Data-quality validation
- Data visualization
- Exploratory Data Analysis

---

## 📁 Repository Structure

```text
Cookie-Company-Interactive-Dashboard/
│
├── README.md
│
├── Cookie Company Interactive Dashboard.xlsx
│
└── screenshots/
    └── dashboard.png
```

> Repository structure may be expanded as additional documentation, screenshots, or supporting files are added.

---

## 🔄 Analytical Workflow

```text
Raw Excel Data
      │
      ▼
Data Quality Audit
      │
      ▼
Identify Duplicate / Overlapping Records
      │
      ▼
Validate Data Types & Business Rules
      │
      ▼
Prepare Analytical Dataset
      │
      ▼
PivotTables / Calculations
      │
      ▼
Interactive Visualizations
      │
      ▼
Excel Dashboard
```

---

## 💡 Key Data-Quality Considerations

This project demonstrates that dashboard development should not begin with visualization alone.

The analytical workflow first considers:

1. **What is the structure of the data?**
2. **Are there missing values?**
3. **Are there duplicate records?**
4. **Are numerical values valid?**
5. **Do business calculations reconcile?**
6. **Are multiple worksheets overlapping?**
7. **What is the appropriate analytical grain?**

This helps prevent inaccurate KPIs and misleading visualizations.

---

## 📌 Project Status

**Status:** 🚧 In Development

The core Excel dashboard and data analysis workflow are being developed as part of a Data Analytics portfolio.

Future improvements may include:

- Additional dashboard KPIs
- More advanced Excel calculations
- Enhanced dashboard interactivity
- Additional business insights
- Data documentation
- Dashboard screenshots
- Further validation and analytical checks

---

## 👤 Author

**Francis Parwez**

Data Analyst

This project is part of my Data Analytics portfolio and demonstrates practical skills in **Excel, data cleaning, exploratory analysis, data visualization, and business intelligence**.
