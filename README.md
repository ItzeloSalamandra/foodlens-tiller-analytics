# FoodLens — Restaurant Intelligence for Tiller by SumUp

> End-to-end analytics pipeline turning 5 years of Paris restaurant POS data into actionable business insights.

## Project Overview

FoodLens analyzes **1M+ real transactions** from 21 Parisian restaurants (2015–2020) using SQL on BigQuery and Python ML to answer the questions every restaurant owner needs answered.

## Key Findings

- **€21.1M** in total revenue analyzed across 5 years
- **COVID-19 impact** clearly captured: revenue dropped 95% in March 2020
- **Friday & Saturday nights** drive peak revenue — critical staffing window
- **5 distinct restaurant profiles** identified via K-Means clustering
- **Cheese Nan + Riz Nature**: lift score of 161 — strongest menu pairing found
- **French holidays** reduce revenue by up to €8,000/day (Prophet model)

## Tech Stack

| Tool | Purpose |
|------|---------|
| BigQuery (SQL) | Data storage, cleaning, KPI queries |
| Python / pandas | Data manipulation |
| scikit-learn | K-Means clustering, PCA |
| Prophet (Meta) | Sales forecasting |
| mlxtend | Market Basket Analysis |
| Plotly / seaborn | Interactive visualizations |

## Analysis Modules

### 1. KPI Dashboard
- Monthly revenue trend (2015–2020)
- Revenue heatmap by day × hour
- Waiter performance matrix

### 2. Menu Intelligence
- Top 15 items by revenue
- Category breakdown

### 3. Restaurant Clustering (K-Means, K=5)
- High-Volume Kiosk
- Classic Brasserie
- Lunch Café
- Night Bar
- Fine Dining

### 4. Sales Forecasting (Prophet)
- 90-day revenue forecast
- Weekly, yearly seasonality + French holidays

### 5. Market Basket Analysis
- Association rules with support, confidence, lift
- Top pairing: Cheese Nan → Riz Nature (lift: 161)

## Dataset

- **Source**: Tiller by SumUp (Le Wagon Data Analytics Bootcamp)
- **Period**: October 2015 – November 2020
- **Tables**: order_data · order_line · payment_data · store_data
- **Size**: 1.28M orders · 3.92M line items · 1.4M payments · 21 stores
- **Location**: Paris, France

## Project Structure
