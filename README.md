

# Executive-Analytics-PowerBI-Solution-

# 🚀 Enterprise Executive Performance Analytics | Power BI

Welcome to the **Executive Performance Analytics** repository. This enterprise-grade Power BI solution bridges robust back-end data engineering with a refined, executive-ready UI/UX interface. Designed to process and analyze historical enterprise transaction data spanning from **2022 to August 2026**, this project demonstrates scalable architecture, automated performance optimization, dynamic security frameworks, and custom analytical controls.

---

## 📽️ Project Walkthrough Video

[Watch Video on LinkedIn](https://lnkd.in/p/e2RXHuKX)

*Click the button above to watch the full interactive walkthrough video on LinkedIn.*

## 📸 Executive-Analytics Dashboard
![Executive Overview Page](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Dashboard.png)

---

## 📌 Business Overview & Problem Statement

Modern enterprise leadership requires high-level visibility alongside the capability to perform granular drill-downs. However, traditional dashboard implementations often suffer from severe performance bottlenecks when scaling over multi-year datasets, security vulnerabilities, or rigid layout structures that clutter the user interface.

**Objective:** Build a high-performance, secure, and interactive executive analytics hub that delivers immediate visibility into core business KPIs (`Sales`, `Profit`, `Orders`, and `Quantity`) while keeping reporting memory footprints minimal and execution lightning-fast.

---

## 🌟 Key Technical Features & Architectural Highlights

### 1. Data Engineering & Query Optimization
* **Incremental Refresh Architecture:** Configured a **5-year data archiving policy** combined with a **1-month active refresh window**. This ensures that historical records are statically preserved in the cloud, while only newly modified transactions are pulled during daily refresh cycles.
* **Query Folding & M-Code Optimization:** Parameterized the ingestion pipeline using `RangeStart` and `RangeEnd` parameters in Power Query. By applying strict date filters directly on the source query, execution is pushed to the database engine (Query Folding), eliminating unnecessary memory overhead in Power BI Desktop during development.

### 2. Enterprise Governance & Granular Security
* **Dynamic Row-Level Security (RLS):** Built a flexible access control system utilizing organizational user identity (`USERPRINCIPALNAME()`). 
* **User Regional Security (`User_Regional_Security`):** Restricts regional managers to view data strictly relevant to their geographic domain (e.g., Alexandria, Cairo, Delta).
* **Executive Security Override:** Built-in administrative logic allowing C-level executives full, unfiltered enterprise-wide visibility across all regions ($27M+ overall volume).

### 3. Front-End Customizations & Interactive Controls
* **Field Parameters (Dynamic Metric Selector):** Replaced multiple static charts with a single interactive visual container. Users can toggle seamlessly between `Total Sales`, `Total Profit`, `Total Orders`, and `Total Quantity`, adjusting visual calculations on the fly.
* **Numeric Range Parameters (Top N Slicer):** Implemented an interactive UI control allowing users to dynamically filter top-performing entities (e.g., Top 3, Top 5, Top 10 Stores) based on selected metrics.

### 4. Design System & UI/UX Standards
* **Soft-Container Visual Layout:** Grouped related metrics into clear visual cards using subtle boundaries and balanced whitespace.
* **Cohesive Executive Palette:** Styled using a professional, modern color system centered around `#48293E` for minimal visual fatigue and maximum readability.

---

## 📐 Data Model & Star Schema Architecture

The analytical core leverages a highly optimized **Star Schema** data model (1-to-Many single-direction relationships) to ensure optimal DAX evaluation speed, minimal memory usage, and accurate aggregation behavior across dimensions.

* **Fact Table:** `FactTransactions` (contains core measures, transactional values, and foreign keys).
* **Dimension Tables:** `DimDate`, `DimStores`, `DimProducts`, `DimRegion`, and `DimSecurity`.

![Data Model](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Model.png)

---

## ⚙️ Detailed Implementation & Technical Screenshots

### 1. Incremental Refresh & Parameter Setup
Configuring `RangeStart` and `RangeEnd` parameters to enforce M-code Query Folding and optimize storage partitions.

| RangeStart Parameter | RangeEnd Parameter | Incremental Refresh Policy |
| :---: | :---: | :---: |
| ![RangeStart](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/RangeStart%20Parameter.png) | ![RangeEnd](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/RangeEnd%20Parameter.png) | ![Incremental Refresh](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Incremental%20Refresh.png) |

---

### 2. Dynamic Row-Level Security (RLS) & Governance
Configuring role definitions, security tables, and deployment to the Power BI Service Workspace.

| Regional RLS Logic | User Regional Security Setup | RLS Live Validation |
| :---: | :---: | :---: |
| ![RLS 1](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/RLS%201.png) | ![User Regional Security](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Incremental%20Refresh.png) | ![RLS 2](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/RLS%202.png) |

| Workspace Environment | InfoSec Architecture | Service Publishing |
| :---: | :---: | :---: |
| ![Workspace](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Workspace.png) | ![InfoSec](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/infoSec%20.png) | ![Publishing](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Publishing%20to%20power%20bi.png) |

---

### 3. Advanced Parameter Design (Field & Numeric Range)
Empowering users with dynamic measure switching and real-time Top N entity filtering.

| Metric Selector Parameter | Top N Range Parameter |
| :---: | :---: |
| ![Metric Selector Parameter](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Metric%20Selector%20Field%20Parameter.png) | ![Top N Parameter](https://github.com/HagerSalahRamadan/Executive-Analytics-PowerBI-Solution-/blob/main/Numeric%20Range%20Parameter%20Top%20N.png) |

---

## 💡 Key Takeaway

> *"High-impact business intelligence isn't just about building dashboards; it’s about engineering resilient data pipelines—blending robust performance and dynamic security with an intuitive executive experience."*

---
## 👤 Author & Contact Information

* **Author:** Hager Salah
* **Role:** Data Analyst / BI Developer
* **Email:** [hagersalah.r39@gmail.com](mailto:hagersalah.r39@gmail.com)
* **LinkedIn:** [Hager Salah](https://www.linkedin.com/in/hager-salah-352803234) 
