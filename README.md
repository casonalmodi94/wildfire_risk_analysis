# Wildfire Risk Prediction (Geospatial Machine Learning)

This project builds a **wildfire risk prediction model** using geospatial data and machine learning.
The goal is to estimate wildfire risk across a study area based on environmental features.

## 🔍 Key Skills Demonstrated

- Python, Pandas, NumPy  
- GeoPandas, spatial data processing  
- Random Forest classification (scikit-learn)  
- Feature engineering for geospatial data  
- Interactive mapping with Folium  
- Exploratory data analysis and model evaluation  

## 📂 Project Structure

```text
wildfire-risk-analysis/
│
├── data/
│   ├── wildfire_samples.csv
│   ├── study_area_boundary.geojson
│   ├── grid_cells.geojson
│
├── notebooks/
│   ├── wildfire_risk_analysis.ipynb
│
├── outputs/
│   ├── grid_cells_with_risk.geojson
│   ├── risk_map_screenshot.png
│
├── requirements.txt
└── README.md

🧠 Model

The model is a Random Forest Classifier trained on:

elevation

vegetation_index

temperature

distance_to_road

Target:
burned (1 = wildfire occurred, 0 = no wildfire)

The model outputs:

Probability of wildfire risk for each grid cell

Discrete risk levels: Low / Medium / High

🗺️ Visualization

An interactive Folium map shows wildfire risk over a 5×5 grid overlaying the study area.

Each cell is color-coded by risk level, with tooltips showing:

Cell ID

Risk probability

Risk level

A screenshot of the map is available in outputs/risk_map_screenshot.png.
