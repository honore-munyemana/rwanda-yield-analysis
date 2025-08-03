# 🇷🇼 Rwanda Crop Yield Analysis (2014–2020)

**Course**: Introduction to Big Data Analytics (INSY 8413)  
**Instructor**: Eric Maniraguha  
**Student**: Munyemana Honore `25594`  
**Submission Date**: July 25, 2025

---

## 🎯 Objective

To analyze agricultural production patterns in Rwanda and categorize crops by yield levels (High, Moderate, Low) using clustering, for improved planning and data-driven decision-making.

---

## 📂 Dataset

- **Source**: [FAOSTAT](https://www.fao.org/faostat/)
- **File**: `Crop_AgroVars_rawdata_Rwanda_2014–2020.csv`
- **Rows**: 1,032  
- **Columns**: 14  
- **Status**: Cleaned and transformed

---

## 🔧 Methodology

### 1. 🧼 Data Preparation (Python)
- Loaded raw FAOSTAT dataset (2014–2020)
- Removed irrelevant or empty rows (e.g., zero production)
- Aggregated total production by crop (`Item`)
- Applied standardization using `StandardScaler`
- Implemented KMeans Clustering to group crops into:
  - Tier 1 – High Yield  
  - Tier 2 – Moderate Yield  
  - Tier 3 – Low Yield
- Created additional feature `Production_Percent`

### 2. 📊 Dashboard Design (Power BI)
- Imported the enhanced dataset
- Created an interactive dashboard with:
  - Bar chart: Crop yield contribution
  - Pie chart: Yield tier distribution
  - Cluster and tier slicers
  - Executive summary section
  - Dynamic filtering and KPI cards

### 3. 💡 Innovation
- Added `Production_Percent` column to show how much each crop contributes to Rwanda's total yield.
- Grouped crop yield patterns using unsupervised learning (KMeans).
- Used Python + Power BI integration for a complete data analysis pipeline.

---

## 📈 Key Insights

- **Bananas** and **Cassava** have the highest yields in Rwanda.
- Most crops fall into **Tier 3 (Low Yield)**.
- Only a few crops such as Beans, Cassava, and Potatoes fall into **Tier 1 (High Yield)**.
- The top 5 crops contribute more than 50% of total production.

---

## 🗂️ Repository Structure

├── data/
│ ├── Crop_AgroVars_rawdata_Rwanda_2014–2020.csv
│ └── rwanda_crop_production_trends.csv
├── screenshots/
│ ├── python_analysis_screens.png
│ ├── powerbi_dashboard_layout.png
│ └── clustering_output.png
├── rwanda_yield.ipynb # Full Python notebook (EDA + clustering)
├── rwanda_yield_analysis.pbix # Final Power BI dashboard
└── README.md # This file


---

## 🧠 Tools & Libraries

- **Python**: Pandas, Scikit-learn, Matplotlib, Seaborn  
- **Power BI**: Visual slicers, pie/bar charts, clustered columns, filters  
- **Clustering Algorithm**: KMeans

---

## ✅ Conclusion

This project demonstrates how big data analytics can help extract meaningful insights from agricultural data. By combining Python and Power BI, we identified Rwanda's most productive crops, grouped them by yield tiers, and built an interactive dashboard to support future decisions in the agriculture sector.
