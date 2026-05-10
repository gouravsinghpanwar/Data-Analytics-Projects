# 📊 Business Performance Dashboard
### Data Analytics Foundation — Course Project
**Submitted by:** Gourav Singh Panwar (AU23B1009)
**Submitted to:** Prof. Dinesh Patel Sir

---

## 🗂️ Project Overview

This repository showcases two end-to-end data analytics projects built as part of the **Data Analytics Foundation** course. Each project demonstrates a different tool and domain, covering the full analytics workflow — from raw data ingestion to interactive dashboard design.

| Project | Tool | Domain |
|---|---|---|
| Used Car Resale Market Analysis | Microsoft Excel | Automobile / Retail |
| IPL Cricket Fantasy Analytics | Power BI | Sports Analytics |

---

## 📁 Repository Structure

```
📦 Business-Performance-Dashboard
 ┣ 📂 Excel-Used-Car-Analysis
 ┃ ┣ 📄 Used_Car_Dashboard.xlsx
 ┃ ┗ 📄 README_Excel.md
 ┣ 📂 PowerBI-Cricket-Analytics
 ┃ ┣ 📄 Cricket_Fantasy_Dashboard.pbix
 ┃ ┗ 📄 README_PowerBI.md
 ┣ 📄 Report.pdf
 ┗ 📄 README.md
```

---

## 📌 Project 1 — Used Car Resale Market Analysis (Microsoft Excel)

### 🎯 Objective
Analyze a large used car sales dataset to extract pricing trends, brand performance, and customer preferences using Excel's data analytics capabilities.

### 📦 Dataset
- **Source:** [Kaggle — Used Car Sales Dataset](https://www.kaggle.com/)
- **Size:** ~60,000 rows × 16 columns
- **Key Attributes:** Brand, Model, Car Type, Transmission, Fuel Type, Year, Kilometers, Owner, State, Price

### 🧹 Data Cleaning & Preparation
- Removed duplicate records and rows with missing/zero price values
- Validated data types across all columns
- **Feature Engineering:**
  - `Car Age` = Current Year − Manufacturing Year
  - `Price Range` → Low / Mid / High segments
  - `KM Category` → Low / Medium / High usage

### 📈 Key KPIs
| KPI | Value |
|---|---|
| Total Cars Listed | 60,207 |
| Average Selling Price | ₹ 0.76 M |
| Average Car Age | 9.05 Years |
| Accidental Cars | 4,739 |
| Total Revenue | ₹ 45,915.58 M |

### 📊 Dashboard Highlights
- **Price Range Distribution** — Bar chart showing Mid-range dominance
- **Top 10 Brands by Sales Volume** — Maruti Suzuki & Hyundai lead
- **State-wise Sales** — Maharashtra & Delhi top regions
- **Car Type vs Average Price** — Luxury & SUVs command premium prices
- **Owner Type Distribution** — 53% First Owners
- **Average Price Trend by Year** — Clear depreciation pattern
- **Fuel Type Distribution** — Petrol 56%, Diesel 30%, CNG 10%

### 💡 Key Business Insights
- **Maruti Suzuki** and **Hyundai** dominate the used car resale market
- **Petrol** cars have the highest resale presence (56%)
- Car prices decrease as car age and kilometers increase (depreciation trend)
- **Non-accidental** cars command significantly higher resale value
- **Mid-range** priced cars show the highest market demand
- **First-owner** vehicles make up over 53% of listings

### 🛠️ Tools Used
`Microsoft Excel` `Pivot Tables` `Excel Charts` `Slicers` `Formulas`

---

## 📌 Project 2 — IPL Cricket Fantasy Analytics (Power BI)

### 🎯 Objective
Build a comprehensive, interactive Power BI dashboard analyzing IPL tournament data (2008–2023) across batting, bowling, fielding, and fantasy dimensions.

### 📦 Dataset
- **Source:** Structured IPL cricket datasets
- **Tables:** Batting, Bowling, Fielding, Fantasy, Match, Team, Player data

### 🗄️ Data Model — Star Schema
```
Fact Tables          Dimension Tables
─────────────        ────────────────
Fact_Batting    ───► Dim_Player
Fact_Bowling    ───► Dim_Team (Batting)
Fact_Fielding   ───► Dim_Team (Bowling)
Fact_Fantasy    ───► Dim_Match
                ───► Dim_Venue
```

### 🧮 DAX Measures Created
- Total Runs, Total Wickets, Matches Played
- Average Strike Rate, Average Economy Rate
- Dot Ball Percentage, Batting & Bowling Averages
- Total Fantasy Points, Fantasy Points per Match
- Dream Team Percentage & Count

### 📊 Dashboard Pages

#### 1. 🏠 Home Page — Tournament Overview
Key KPIs: **14M** Fantasy Points | **305K** Total Runs | **11K** Wickets | **1K** Matches

#### 2. 🏏 Batting Analysis
- Top 10 batters by runs (Virat Kohli leads with 7.3K)
- Batting consistency %, average strike rate (109.30), total boundaries (39K)
- Season-wise runs trend and boundary analysis

#### 3. 🎳 Bowling Analysis
- Top 10 bowlers by wickets (Yuzvendra Chahal leads with 187)
- Average economy (8.36), dot ball % (0.38), bowling average (28.76)
- Team-wise wicket distribution and economy rate comparison

#### 4. ⭐ Dream Team Analysis
- Top fantasy earners (Virat Kohli — 167K points)
- Dream Team % (0.50), Dream Team Count (173K)
- Team contribution to fantasy points

### 💡 Key Insights
- **Virat Kohli** leads in both runs (7.3K) and fantasy points (167K)
- **MI, SRH, CSK** are the strongest teams in bowling wicket counts
- Fantasy points trend shows a significant spike post-2015
- Only **18.89%** of player-match instances qualify as Dream Team selections

### 🛠️ Tools Used
`Power BI Desktop` `Power Query` `DAX` `Star Schema Modeling`

---

## ⚖️ Comparative Analysis — Excel vs Power BI

| Aspect | Microsoft Excel | Power BI |
|---|---|---|
| Dataset Size | Small to Medium | Large & Multi-table |
| Data Model | Flat / Pivot-based | Star Schema |
| Calculations | Formulas & Pivot | DAX Measures |
| Interactivity | Limited (Slicers) | High (Drill-through, Cross-filter) |
| Scalability | Limited | Enterprise-ready |
| Learning Curve | Low | Moderate |
| Best For | Quick EDA & Prototyping | Advanced BI & Storytelling |

**Takeaway:** Excel is ideal for quick, accessible analysis on moderate datasets. Power BI is the right tool when scalability, interactivity, and complex data modeling are required.

---

## 🏁 Conclusion

Both projects collectively demonstrate the ability to:
- Select the right tool for the right analytical problem
- Perform end-to-end analytics from raw data to executive dashboards
- Extract actionable business and sports insights through structured data modeling
- Design interactive dashboards for both technical and non-technical audiences

---

## 📬 Contact

**Gourav Singh Panwar**
Student ID: AU23B1009
📧 *[gourav.panwar@avantika.edu.in]*
🔗 *www.linkedin.com/in/gourav-singh-panwar-ba614727a*
