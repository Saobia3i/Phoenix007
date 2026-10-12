


# 🔥 FireSync: Harmonization of MODIS and VIIRS Hot Spots

![NASA Space Apps Challenge 2026](https://img.shields.io/badge/NASA_Space_Apps-2026-0B3D91?style=for-the-badge&logo=nasa)
![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)

> A unified, AI-driven burning activity calendar bridging the gap between historical MODIS and VIIRS satellite active fire data.

---

## 📖 Table of Contents
- [Overview](#overview)
- [The Challenge](#the-challenge)
- [Our Solution](#our-solution)
- [Data Sources](#data-sources)
- [Tech Stack](#tech-stack)
- [Architecture & Methodology](#architecture--methodology)
- [Local Installation](#local-installation)
- [Team Phoenix007](#team-phoenix007)

---

## 🌍 Overview
Understanding how burning activity is distributed across our planet over time is critical for anticipating crises and improving fire response[cite: 5]. While satellites have tracked intense active fire hotspots for decades, the historical record is fragmented across different sensors[cite: 5]. This project harmonizes data from MODIS and VIIRS sensors to create a continuous, reliable historical baseline of global fire activity.

## 🎯 The Challenge
**Challenge:** Harmonization of MODIS and VIIRS Hot Spots[cite: 5].  
**Problem Statement:** The historical record of satellite-detected fires cannot be compared directly across different sensors without a consistent picture of when and where burning has occurred[cite: 5]. This fragmentation hinders the ability of land managers and early warning systems to examine historical trends and critical burning periods[cite: 5].

## 💡 Our Solution
We built an interactive, AI-powered platform that standardizes and merges decades of thermal anomaly data into a unified "burning activity calendar"[cite: 5]. 

**Key Features:**
*   **Data Harmonization Engine:** A machine learning pipeline that normalizes the spatial and temporal differences between MODIS (1km resolution) and VIIRS (375m resolution).
*   **Burning Activity Calendar:** An interactive UI allowing users to filter historical fire data by region, time period, and intensity[cite: 5].
*   **Early Warning Analytics:** Predictive insights that empower emergency responders and scientists to identify unusual environmental conditions[cite: 5].

---

## 🛰️ Data Sources
We utilize NASA Earth observation data to power our harmonization engine:
*   **NASA FIRMS API:** Primary data distribution system for near real-time and historical fire data.
*   **MODIS (Moderate Resolution Imaging Spectroradiometer):** Terra and Aqua satellite data for long-term historical baselines.
*   **VIIRS (Visible Infrared Imaging Radiometer Suite):** Suomi NPP, NOAA-20, and NOAA-21 satellite data for high-resolution active fire detection.

---

## 🛠️ Tech Stack
*(Note: Update this section based on the exact tools your team uses)*
*   **Backend & Data Processing:** Python, Pandas, GeoPandas, FastAPI
*   **Machine Learning:** Scikit-Learn / PyTorch (for harmonization models)
*   **Frontend:** React.js, Tailwind CSS, Mapbox GL JS / Leaflet (for geospatial visualization)
*   **Deployment:** Docker, AWS / Google Cloud

---

## ⚙️ Architecture & Methodology
1.  **Data Ingestion:** Automated scripts fetch historical datasets via NASA FIRMS.
2.  **Preprocessing & Cleaning:** Handling missing values, filtering cloud-cover false positives, and standardizing timestamp formats.
3.  **Spatial Harmonization:** Using spatial clustering (e.g., DBSCAN) and regression models to bridge the gap between MODIS's 1km pixels and VIIRS's 375m pixels.
4.  **API Delivery:** A RESTful API serves the harmonized data to the frontend calendar interface.

---

## 🚀 Local Installation

### Prerequisites
*   Python 3.10+
*   Node.js v16+
*   NASA FIRMS API Key

### Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/your-repo/firesync-phoenix007.git](https://github.com/your-repo/firesync-phoenix007.git)
   cd firesync-phoenix007

```

2. **Backend Setup:**
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt

```


3. **Environment Variables:**
Create a `.env` file in the root directory and add your keys:
```env
FIRMS_API_KEY=your_api_key_here

```


4. **Run the Application:**
```bash
uvicorn main:app --reload

```



---

## 👥 Team Phoenix007

We are **Team Phoenix007**, an innovative AI team from Bangladesh participating in the 2026 NASA Space Apps Challenge.

* **Saobia Islam** - Team Leader


* **Mashrur Rahman** - Software Engineer


* **Ahnuf Karim Chowdhury** - Data Scientist


* **Chowdhury Ajmayeen Adil** - Machine Learning Engineer


* **Nahid Asef** - Frontend Developer



---

*Built with ❤️ for the 2026 NASA Space Apps Challenge.*


