<div align="center">

# 🗺️ Geo-Statistical Data Visualization: Regional Insights via Interactive Mapping

![Language](https://img.shields.io/badge/Language-Python_3-blue?style=for-the-badge&logo=python&logoColor=white)
![Environment](https://img.shields.io/badge/Environment-Google_Colab-orange?style=for-the-badge&logo=googlecolab&logoColor=white)
![Libraries](https://img.shields.io/badge/Libraries-Folium_%7C_Pandas_%7C_Seaborn-green?style=for-the-badge)
![Data Source](https://img.shields.io/badge/Data_Source-BPS_Indonesia-darkblue?style=for-the-badge)

<p align="center">
  <strong>A data science project focused on translating official statistical datasets into interactive charts and geospatial heatmaps.</strong>
</p>

[Project Overview](#-project-overview) • [Analysis Objectives](#-analysis-objectives) • [Tech Stack](#-technology-stack) • [Repository Structure](#-repository-structure) • [Visualizations & Insights](#-visualizations--insights)

</div>

---

## 📖 Project Overview

This repository contains a comprehensive data analytics and visualization project titled **"Visualisasi Data Statistik ke Peta" (Statistical Data Visualization onto Maps)**, developed by **Group 4**. 

The project focuses on extracting macro-economic and social indicators from the **Central Bureau of Statistics (BPS)** and transforming them into intuitive, multi-dimensional visual mediums. It explores two distinct thematic datasets across different regions:
1. **Registered Job Vacancies** by Regency/Municipality and Gender in East Java Province (2022 Data).
2. **Gender Inequality Index (IKG - Indeks Ketimpangan Gender)** across Regencies/Municipalities in West Java Province.

---

## 🎯 Analysis Objectives

The primary goal of this study is to implement programmatic geographical mapping to uncover structural regional insights. The pipeline accomplishes:
- 📊 **Geographical Distribution Tracking:** Visualizing the density and spread of employment opportunities in East Java.
- ⚖️ **Social Inequality Mapping:** Dissecting the Gender Inequality Index (IKG) disparities throughout West Java to identify regions requiring development focus.
- 🗺️ **Interactive Heatmap Generation:** Replacing traditional flat data tables with dynamic, interactive maps that allow effortless spatial data interpretation.

---

## 🛠️ Technology Stack

The data processing pipeline and visualization engine are entirely engineered in Python inside a modular workspace:

| Tool / Library | Functional Purpose |
| :--- | :--- |
| **Pandas** | Structural data ingestion, metadata stripping, string cleaning, type casting, and filtering. |
| **Matplotlib** | Core figures layout creation, axis labeling, tight-layout wrapping, and grid rendering. |
| **Seaborn** | High-level statistical plotting, multi-variable color sorting, and conditional categorizations. |
| **Folium** | Leaflet.js-backed engine for map container setup, custom coordinate plotting, and responsive marker bounding. |
| **Folium.plugins (HeatMap)** | Generating dynamic density layers to represent statistical weight over precise coordinates. |

---

## 📂 Repository Structure

```text
StatisticalDataVisualization/
│
├── 📄 StatisticalDataVisualization_Kelompok4.ipynb  # Core Jupyter Notebook detailing the entire data pipeline
└── README.md                                          # Main repository documentation
```

## 📊 Visualizations & Insights

The data processing pipeline filters raw datasets through specific structural data cleaning operations, such as removing metadata noise, casting structural datatypes to numeric floats, dropping empty null fields, and filtering regional aggregates to prepare them for seamless analytical layers.

### 1. Gender Inequality Index (IKG) Analysis – West Java
*   **Statistical Chart Insights:** The Seaborn horizontal bar chart dynamically sorts regional metrics from highest to lowest inequality[cite: 4]. Further conditional slicing isolates the top 10 highest IKG regions to highlight major structural gaps[cite: 4]. Through this visualization, **Cianjur** ($0.555$) and **Bogor** ($0.547$) are pinpointed as the regions with the highest gender developmental gaps[cite: 4]. Conversely, **Kota Cimahi** preserves the lowest gap ($0.166$) against a West Java regional average of $0.370$[cite: 4].
*   **Interactive Heatmap Mapping:** Utilizing geographic coordinates embedded via `folium`, the map engine sets up dynamic rendering over a clean map layout[cite: 4]. Custom circular markers are bound with responsive hover tooltips and interactive popups to display quick contextual data upon user clicks[cite: 4].

### 2. Job Vacancy Distribution Analysis – East Java
*   **Pipeline Infrastructure:** Cleans multi-tier header sheets into a structured dataframe containing isolated, cleanly cast columns for male, female, and overall job vacancy statistics[cite: 4].
*   **Macro Distribution Mapping:** Generates sorted categorical comparisons showing absolute labor request variations across diverse industrial municipal hubs in East Java[cite: 4].

---

## 🎓 Author

**Cesya Aulia Ramadhani**  
*Applied Science Undergraduate Student in **Management Informatics** — Universitas Negeri Surabaya*[cite: 4]
