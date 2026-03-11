# Hourly Energy Consumption Forecasting

## Overview
Machine learning model to forecast hourly electricity demand using real grid data from PJM Interconnection — a regional transmission organization serving 65 million people across the US east coast.

## Motivation
Built to explore ML applications in power systems — specifically how data-driven models can support power dispatch optimization and grid management, relevant to modern smart grid research.

## Dataset
- Source: PJM Interconnection (via Kaggle)
- 145,366 hourly energy readings from 2002–2018
- Features: hour of day, day of week, month, year

## Model
- Algorithm: XGBoost Regressor
- Train/test split: 80/20
- RMSE: ~2,958 MW (~8-10% error on a 30,000–40,000 MW grid)

## Results
The model successfully learned seasonal and daily demand patterns:
- Summer peaks driven by air conditioning load
- Winter secondary peaks from heating
- Daily cycles with overnight demand drops

## Tools
Python, Pandas, XGBoost, Scikit-learn, Matplotlib
