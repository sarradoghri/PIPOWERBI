# CompareIt Power BI Dashboards

This repository contains the Power BI dashboards and related documentation for the **CompareIt Business Intelligence project**. The platform provides price comparison insights across three main categories:

- **Magasin (Store) Dashboard**  
- **Hotel Dashboard**  
- **Vol (Flight) Dashboard**

---

## Dashboards Overview

### 1. Magasin Dashboard  
- Focuses on product price comparison and responsible consumption (aligned with SDG 12).  
- Includes interactive visualizations, KPIs, and price trend analyses.  
- Integrates **Machine Learning models** to provide:  
  - Product recommendations using TF-IDF and cosine similarity.  
  - Budget-based filtering for personalized suggestions.  
  - Price prediction models to forecast future prices.  
  - (Optional) Customer segmentation for targeted insights.  

> **Note:** Machine learning models are implemented exclusively for the Magasin dashboard to enhance user experience and decision support.

### 2. Hotel Dashboard  
- Visualizes hotel pricing trends and market competitiveness (aligned with SDG 8).  
- Provides economic growth insights via occupancy, pricing, and booking patterns.  
- Does not currently include machine learning components.

### 3. Vol (Flight) Dashboard  
- Analyzes flight price trends and infrastructure-related metrics (aligned with SDG 9).  
- Offers time series forecasts using classical statistical models (SARIMA).  
- Machine learning is not applied to this dashboard in the current phase.

---

## Machine Learning Module Summary (Magasin Only)

- **Recommendation System:** TF-IDF vectorization + Cosine similarity for personalized product suggestions.  
- **Budget Filtering:** Ensures recommended products fall within the user’s budget.  
- **Price Prediction:** Regression models to forecast product prices based on historical data.  
- **Customer Segmentation (Optional):** Random Forest classifier categorizing shopper types.  
- **Future Enhancements:** Anomaly detection and deep learning models for improved forecasts.

---

## Data Preparation and Integration

- Data collected via APIs and CSV files, processed with ETL pipeline.  
- Data stored in SQL Server Data Warehouse designed with star schema.  
- Power BI dashboards connected via DirectQuery and scheduled refreshes.

---

## Deployment

- Dashboards embedded in web portals using Power BI Embedded.  
- Role-level security implemented for personalized data views.
