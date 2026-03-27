# 🦠 COVID-19 Trend Analysis & Geographic Spread (2020)
**Course:** STAT 674 – Applied Database Management | University of Delaware  
**Team:** Sarah Donaldson, Greta Schieroni, Rahul Chauhan  
**Tools:** SAS (PROC SQL, PROC SGPANEL, PROC SGPLOT)

---

## 📌 Project Overview
Analyzed COVID-19 case and death data across four major global regions in 2020 to identify geographic spread patterns, wave timing, and the relationship between infection rates and mortality.

---

## ❓ Research Questions
1. Which countries in Asia, Europe, South America, and Africa had the highest reported cases in 2020?
2. Is there a correlation between infection rate and death rate across regions?
3. How did the death-to-case ratio evolve monthly within each region?
4. What demographic factors (median age, population, % aged 65+) correlate with COVID-19 severity?

---

## 📊 Dataset
- **Source:** Our World in Data – COVID-19 dataset
- **Scope:** Top 5 countries per region (Asia & Europe; South America & Africa)
- **Time range:** January – December 2020
- **Key variables:** `total_new_cases`, `total_new_deaths`, `population`, `median_age`, `aged_65_older`

---

## 🛠️ SAS Procedures Used
| Procedure | Purpose |
|---|---|
| `PROC SQL` | Data querying, filtering top-5 countries per region |
| `PROC SGPANEL` | Multi-panel time series charts (cases & deaths by country) |
| `PROC SGPLOT` | Bubble plots, line charts for death-to-case ratio |

---

## 📈 Key Findings

### Asia & Europe
- **India** had the highest new cases (~2.5M monthly peak)
- **Iran** had the highest death rate (%) relative to infection rate
- Death-to-case ratios declined across all countries as the year progressed — suggesting improved treatment protocols

### South America & Africa
- **Brazil** had the highest total cases (7,448,560) and deaths (190,488) — driven largely by its much larger population
- **Peru** had a significantly higher death-to-case ratio than all other countries in the region, peaking mid-year
- No strong universal correlation between raw case counts and death counts across countries

### Heat Map Analysis
- Population size was the dominant differentiating factor for total cases
- No significant cross-country differences in median age or proportion aged 65+ among the top 5 countries

---

## 📁 Repository Structure
```
├── sas_code/           # All .sas scripts (PROC SQL queries, visualizations)
├── output/             # Exported charts (PNG/PDF from SAS)
├── data/               # Raw input CSV files
├── presentation/       # Slide deck (PDF)
└── README.md
```

---

## 🖼️ Visualizations Produced
- Monthly COVID-19 cases & deaths — multi-panel by country (Asia/Europe)
- Monthly COVID-19 cases & deaths — multi-panel by country (South America/Africa)
- Bubble plot: Infection rate vs. Death rate by country
- Line chart: Monthly death-to-case ratio over time
- Heat map: COVID-19 impact & demographics by country

---

## 🔧 How to Run
Open the `.sas` files in SAS Studio or SAS Enterprise Guide. Ensure the input CSV data files are placed in the `data/` folder and update the `libname` path accordingly.
