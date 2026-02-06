<div align="center">

# 🌿 Eco-Traffic Seattle
### *Smart City Traffic Prediction via Multi-Source Data Enrichment*

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com)
[![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)](https://mlflow.org)

---



**Predicting urban congestion levels (Fluid, Moderate, Critical) by merging SDOT traffic flow data with real-time scraped weather and news insights.**

</div>

## 👥 Authors
> Developed by **Mohamed Raed Bouhali** & **Ilef Ben Hassen** > *Module: Python for Data Science 2*

---

## 🎯 Project Overview
The goal is to move beyond static data. By enriching historical traffic logs with contextual data (weather conditions and local news), we provide a dynamic prediction engine for Seattle's road networks.

### ⚙️ Functional Specifications
<table width="100%">
  <tr>
    <td width="50%">
      <h4>📥 Data Ingestion</h4>
      Automated 2022 weather data collection and incident extraction via <b>BeautifulSoup</b> & <b>Selenium</b>.
    </td>
    <td width="50%">
      <h4>🧠 Predictive Core</h4>
      Geospatial and temporal classification using <b>XGBoost</b> and <b>Random Forest</b>.
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h4>💻 User Interface</h4>
      Interactive <b>React</b> Dashboard with real-time <b>Leaflet</b> maps for future state visualization.
    </td>
    <td width="50%">
      <h4>🚀 Service Access</h4>
      High-performance <b>FastAPI</b> endpoints for unit and batch predictions.
    </td>
  </tr>
</table>

---

## 🛠 Technical Stack

### 🧪 Data Science & ML
- **Scraping:** BeautifulSoup & Selenium (News/Weather extraction).
- **Processing:** `Pandas`, `NumPy`, and Feature Engineering for seasonality.
- **Sampling:** **SMOTE** (Synthetic Minority Over-sampling Technique) to handle critical congestion imbalance.
- **Tracking:** **MLflow** for experiment logging and model versioning.

### 🌐 Software Architecture
- **Backend:** FastAPI (Python) with Batch processing capabilities.
- **Frontend:** React + Vite + Leaflet.js.
- **Infrastructure:** Containerization via **Docker** & **Docker-Compose**.



---

## 📌 Deliverables
- [x] **Documented Source Code:** Clean, modular Python & React code.
- [x] **Dockerized Environment:** One-command deployment (`docker-compose up`).
- [x] **Live Dashboard:** Full visualization of Seattle traffic predictions.

---

<div align="center">
  <sub>Built with ❤️ for Seattle Smart Mobility</sub>
</div>
