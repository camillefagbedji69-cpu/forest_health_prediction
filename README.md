# NDVI Forecasting in the Lama Forest

## 📌 Context & Overview
The Lama Classified Forest is a critical biodiversity hotspot in Benin. Monitoring its health is vital for conservation efforts amidst climate change. This project focuses on predicting the **Normalized Difference Vegetation Index (NDVI)**—a satellite-derived proxy for vegetation vigor—to anticipate ecosystem shifts.

## 🎯 Objectives
* **Trend Analysis:** Quantify interannual and seasonal NDVI variations over two decades.
* **Predictive Modeling:** Develop a robust machine learning baseline for vegetation state forecasting.
* **Remote Sensing Integration:** Explore the synergy between Earth Observation data and predictive analytics.

## 📊 Data Description
* **Source:** Google Earth Engine (MODIS/Landsat composites).
* **Metric:** Monthly Mean NDVI.
* **Timeframe:** January 2000 – February 2023 (23 years).
* **Dataset Size:** 277 observations.

## 🛠️ Methodology & Tech Stack
* **Language:** Python 🐍
* **Platform:** Google Earth Engine (Extraction) & VS Code (Modeling).
* **Libraries:** `Scikit-learn`, `Pandas`, `Matplotlib`, `Statsmodels`.

### Workflow:
1. **Data Acquisition:** Time-series extraction via Google Earth Engine.
2. **Time-Series Decomposition:** Breaking down the signal into **Trend**, **Seasonality**, and **Residuals**.
3. **Feature Engineering:** Creating lagged variables to capture temporal dependencies.
4. **Model Selection:** Implementation of a **Random Forest Regressor**.
5. **Evaluation:** Performance assessment using **RMSE**.

## 🚀 Key Results
* **Ecosystem Resilience:** The mean annual NDVI consistently remained above 0.50, indicating a stable and well-preserved forest cover.
* **Seasonal Dynamics:** * **Peak:** March–June (Primary rainy season).
    * **Trough:** December–February (Major dry season).
* **Model Performance:** The Random Forest model achieved a **RMSE of 0.0467**, demonstrating strong generalization capabilities for a baseline exploratory model.

## 🔮 Perspectives for Improvement
* **Advanced Architectures:** Transitioning from Random Forest to specialized temporal models like **SARIMA** or **LSTM** (Deep Learning).
* **Multivariate Analysis:** Integrating exogenous bioclimatic variables (Rainfall, Temperature, Soil Moisture) to enhance predictive accuracy.
* **Spatial Forecasting:** Moving from point-based mean NDVI to pixel-wise spatial prediction.
