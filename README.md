# Haifa Eco Pulse: Spatial-Temporal Ecological Dashboard

An analytical dashboard designed for environmental researchers, urban planners, and the public to perform spatial-temporal monitoring and cross-referencing between air pollution indices and vegetation health across the city of Haifa and the Carmel ridge.

---

## 👥 Team: Nature Bytes

Developed as part of the Ecological Modeling Laboratory Course, Spring 2026.

---

## 📌 Project Overview

Haifa is a complex urban and industrial hub characterized by a combination of industrial and transportation emissions and a surrounding urban-forest ecosystem. **Haifa Eco Pulse** acts as an ecological health monitor by tracking and analyzing the correlation between Nitrogen Dioxide ($NO_2$) tropospheric pollution and the Normalized Difference Vegetation Index (NDVI).

By synthesizing remote sensing data, the dashboard maps ecological dynamics and predicts potential ecosystem degradation or recovery trends.

---

## DEMO
https://github.com/user-attachments/assets/47e33949-f774-42a9-86d7-058b1d42eef1

---

## 🛠️ System Architecture & Features

* **Interactive GIS Mapping:** Displays a dynamic, layered map of Haifa with $NO_2$ and NDVI spatial distributions fetched via the Google Earth Engine (GEE) API.
* **Temporal Slider:** Multi-tab interface featuring a time slider component allowing users to slide through chronological blocks to observe environmental variations over time.
* **Local Data Caching:** Optimizes performance by storing historical satellite queries locally into structured CSV files, minimizing GEE API server overhead and keeping chart loading latency under 2 seconds.
* **Statistical Insights Hub:** Computes trend lines and executes continuous analytical tests to output explicit, interactive mathematical correlations directly inside the UI.

---

## 📊 Scientific Methodology

The system relies on an ecosystem framework modeled after **Odum’s systems ecology**. It monitors energy/matter processing loops—tracking how human industrial inputs (fossil fuels/$NO_2$) interact with natural inputs (solar radiation) to dynamically regulate or degrade vegetation tissue over time.

### Statistical Modeling
1. **Pearson & Spearman Correlation ($r$):** Used to determine the strength and direction of the linear relationship between continuous variables ($NO_2$ and $NDVI$).
2. **One-Way ANOVA & Tukey’s HSD:** Executed to isolate macro seasonal shifts in mean pollution levels, evaluating if summer months exhibit higher concentration thresholds due to topographic inversion layers.
3. **Kriging Spatial Interpolation:** An advanced geo-statistical prediction technique that maps a continuous surface of air quality and biological strain across unsampled zones of Haifa based on spatial continuity.

---

## 💻 Tech Stack & Environment

* **Frontend Dashboard:** Python (Streamlit/Dash), HTML5, CSS3.
* **Geospatial Processing:** Google Earth Engine (GEE) API, RAG Architecture.
* **Data Science & Statistics:** `scikit-learn`, `scipy.stats`, `pandas`, `numpy`, `statsmodels`.
* **Database & Caching:** Local CSV/Parquet files for high-speed edge rendering.

