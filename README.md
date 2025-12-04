#  Bike Fleet Intelligence:Pattern Mining, User Clustering \& Predictive Analytics for Bike Sharing

## Project Overview

This project analyzes 17.5 million NYC Citi Bike trips from 2018 to discover travel patterns, segment users, and forecast bike demand. We integrate real time weather data to understand environmental impacts on bike sharing behavior.

## Objectives

1. **Frequent Pattern Mining** – Discover popular routes and commute patterns using the Apriori algorithm
2. **User Segmentation** – Cluster riders based on behavior using Hierarchical Clustering
3. **Demand Forecasting** – Predict hourly pickups/dropoffs using XGBoost with weather features

## Dataset

- **Source:** [NYC Citi Bike System Data](https://citibikenyc.com/system-data)
- **Period:** January – December 2018
- **Size:** ~17.5 million trips (~2GB)
- **Weather:** Open-Meteo ERA5 Historical API

## Methods

| Task | Algorithm | Course Topic |
|------|-----------|--------------|
| Pattern Mining | Apriori | Frequent Itemsets |
| User Clustering | Hierarchical (Ward) |  General Clustering |
| Demand Forecasting | XGBoost | External Topic |

### Evaluation Metrics
- **Clustering:** Davies-Bouldin Index, Silhouette Score
- **Forecasting:** MAE, RMSE

## Key Results

- **Apriori:** Identified 15+ frequent route patterns and commute behaviors
- **Clustering:** Segmented users into 5 distinct behavioral groups
- **Forecasting:** XGBoost with weather features achieved ~15% improvement over baseline

## Project Structure
```
├── Final_Project_new_version.ipynb  # Main notebook
├── Parallel Processing/             # Parallel processing scripts
├── Data_source.txt                  # Dataset download link
├── README.md
└── .gitignore
```

## Installation
```bash
pip install pandas numpy requests matplotlib seaborn mlxtend scipy scikit-learn xgboost
```

## Usage

1. Clone the repository
2. Run `Final_Project_new_version.ipynb`
3. The notebook will automatically download the dataset (~2GB)