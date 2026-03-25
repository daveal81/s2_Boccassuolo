# s2_Boccassuolo

# 🌍 Boccassuolo Landslide Monitoring with Google Earth Engine

This project uses **Google Earth Engine (GEE)** and **geemap** to perform a time-series analysis of the Boccassuolo landslide area. By leveraging **Sentinel-2 Surface Reflectance** data, the script visualises terrain changes across multiple dates in 2025.

---

## 🛰️ Overview

The workflow automates the retrieval of satellite imagery for a specific set of coordinates (AOI) and applies cloud-filtering to ensure high-visibility monitoring. It is designed to help researchers and geologists observe landslide dynamics over time through an interactive map interface.

### Key Features
* **Multi-temporal Analysis:** Loads imagery for 9 specific dates between March and July 2025.
* **Automated Pre-processing:** Filters for cloud cover (<80%) and clips imagery to the study area.
* **Interactive Visualization:** Uses `geemap` to toggle between different satellite passes.
* **Vector Overlays:** Displays the Area of Interest (AOI) and landslide boundaries with custom styling.

---

## 🛠️ Setup & Installation

To run this notebook/script, you will need a Google Earth Engine account. If you don't have one, [sign up here](https://earthengine.google.com/).

### 1. Install Dependencies
If you are running this locally or on GitHub Codespaces, you must install the Earth Engine API and `geemap`:

```bash
pip install earthengine-api geemap
