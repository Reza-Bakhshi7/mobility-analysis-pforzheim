# 🚲 Mobility Analysis Pforzheim — GIS & Data Visualization

A spatial analysis of urban mobility infrastructure in Pforzheim (Baden-Württemberg), evaluating the accessibility and distribution of public transport, bikesharing, and e-scooter services across the city.

**Course:** SUM 3 III.1 — Data Analysis and Visualization  
**University:** HfWU Nürtingen-Geislingen  
**Date:** August 2025

---

## 📋 Overview

This project uses GIS techniques to assess how well different parts of Pforzheim are served by sustainable mobility options. A special focus is placed on the accessibility challenges around **Hochschule Pforzheim**, which serves thousands of students daily but lies outside the city's multimodal core.

### Key Findings
- **61% of trips** in Pforzheim are made by private car (MiD 2017)
- Only **8% public transport** and **6% bicycle** mode share
- Multimodal accessibility is heavily concentrated in the city center
- The university's main campus has **no coverage** in the 200m multi-modal access zone

---

## 🗺️ Maps Produced

| Map | Description |
|-----|-------------|
| Overview Map | City boundary, districts, street network |
| Bus Stops | Distribution of public transport nodes |
| Bike & E-Scooter Sharing | Spatial distribution of shared micro-mobility |
| 10-Minute Walk Isochrone | Walking accessibility from city center |
| Heatmap | Concentration of shared mobility services |
| Multi-Modal Access Zone | Areas with bus + bike + scooter within 200m |
| City Area / Mesh Analysis | Road-based fragmentation of urban space |

---

## 🔧 Methods & Tools

- **QGIS** — All spatial analysis and map production
- **Buffer Analysis** — 200m around bus stops, bike & scooter stations
- **Heatmapping** — Service concentration visualization
- **Network Analysis** — 10-minute walking isochrone (4 km/h)
- **Mesh/Fragmentation Analysis** — Road-based area segmentation (102 zones)
- **Coordinate System:** EPSG:25832 (ETRS89 / UTM zone 32N)

---

## 📊 Data Sources

| Dataset | Source |
|---------|--------|
| City boundary & street network | [Geofabrik / OpenStreetMap](https://download.geofabrik.de) |
| Bikesharing stations BW | [MobiData BW](https://mobidata-bw.de/dataset/bikesh) |
| E-Scooter sharing stations BW | [MobiData BW](https://mobidata-bw.de/dataset/escootch) |
| Radnetz BW (cycle network) | [MobiData BW](https://mobidata-bw.de/dataset/radnetz-bw) |
| Modal split data | [Mobilität in Deutschland 2017](https://www.mobilitaet-in-deutschland.de) |
| Basemaps | OpenStreetMap, TopPlusOpen WMS (BKG) |

---

## 📁 Repository Structure

```
mobility-analysis-pforzheim/
├── README.md
├── maps/                    # Exported map images (PNG/PDF)
│   ├── 01_overview.png
│   ├── 02_bus_stops.png
│   ├── 03_bike_scooter_sharing.png
│   ├── 04_walking_isochrone.png
│   ├── 05_heatmap.png
│   ├── 06_multimodal_access_zone.png
│   └── 07_city_area_mesh.png
├── qgis/                    # QGIS project file(s)
│   └── pforzheim_mobility.qgz
├── data/                    # Raw/processed data (or links)
│   └── README.md            # Data source descriptions
└── docs/
    └── seminar_paper.pdf    # Full seminar paper
```

---

## 📌 Recommendations

1. Add bike and scooter stations near Hochschule Pforzheim (Tiefenbronner Straße)
2. Introduce micro-mobility partnerships for the university (student tariff)
3. Improve bus frequency in the southern districts
4. Use spatial analysis for future mobility planning to prevent exclusion

---

## 📄 License

This project was created for academic purposes at HfWU Nürtingen-Geislingen. Data sources are credited above.

---

## 👤 Author

**Mohammadreza (Reza) Bakhshi**  
M.Sc. Sustainable Mobilities — HfWU Nürtingen-Geislingen  
[LinkedIn](https://www.linkedin.com/in/m-rezabakhshi) · [GitHub](https://github.com/Reza-Bakhshi7)
