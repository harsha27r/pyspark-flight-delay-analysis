# ✈️ US Flight Delay Analysis with PySpark

## Overview
Large-scale analysis of **5.8 million US domestic flight records** using Apache PySpark on Databricks. This project explores delay patterns, identifies the worst-performing airlines and routes, and breaks down cancellation causes across the entire 2015 US flight dataset.

## Tools & Technologies
- **Apache PySpark** — distributed data processing
- **Databricks** — cloud execution environment
- **Delta Lake** — results saved as Delta tables
- **Python** — data manipulation and analysis

## Dataset
- Source: [US DOT Flight Delays (Kaggle)](https://www.kaggle.com/datasets/usdot/flight-delays)
- 5,819,415 flight records
- 38 columns including departure/arrival delays, cancellation reasons, airline codes, and route info

## Analysis Performed
1. **Dataset overview** — total flights, cancellations, diversions
2. **Worst airlines by average arrival delay**
3. **Worst routes by average departure delay** (min. 100 flights)
4. **Cancellation breakdown by reason** (A=Airline, B=Weather, C=NAS, D=Security)
5. **Delay causes breakdown** — weather vs airline vs air system vs late aircraft
6. **Delays by day of week** — which days are worst for travel

## Key Findings
- Over 89,000 flights were cancelled (1.5% of total)
- Airline-caused delays and late aircraft are the leading delay contributors
- Fridays and Thursdays tend to have the highest average delays
- Certain hub-to-hub routes consistently show the worst departure delays

## How to Run
1. Sign up for [Databricks Community Edition](https://community.cloud.databricks.com) (free)
2. Upload `flights.csv` from the Kaggle dataset and create a table
3. Import the notebook and run all cells
