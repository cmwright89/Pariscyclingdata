# Paris Cycling Traffic Analysis

## Project Overview
This repository contains my contributions to a collaborative data analysis project examining cycling traffic patterns in Paris from September 2023 to June 2024. The full project was conducted as part of the Data Analyst Bootcamp by DataScientest (September 2024 Cohort) in partnership with Amal MOHAMED and Dirk Eisermann.

## My Contributions
This repository specifically includes the code I personally developed for the project:

- **Data Visualization**: Contributed specific visualizations to identify cycling patterns across Paris (note: teammates also produced additional visualizations not included in this repository)
- **HDBSCAN Clustering**: Implemented density-based spatial clustering to identify natural groupings of cycling counters
- **Log-transformed HDBSCAN Analysis**: Applied log transformation to skewed data for improved cluster detection

## Project Background
In 2021, Paris introduced the "Plan Velo: Act 2" as part of their vision to become a fully bikeable city. The city installed cyclist counting meters throughout Paris to monitor usage. Our project analyzed this data to:

1. Identify high and low traffic cycling routes
2. Evaluate the impact of the 2024 Olympic and Paralympic Games on cycling traffic
3. Use unsupervised learning to identify traffic pattern distributions
4. Create a supervised model to predict afternoon cyclist counts from morning data

## Data Sources
- Main dataset: Hourly cyclist counts from counters across Paris (from opendata.paris.fr)
- Secondary dataset: Street address information for arrondissement classification

## Key Findings
- Distinct cycling corridors were identified, including high-traffic north-south and east-west routes
- Weekday cycling traffic significantly exceeds weekend traffic, suggesting commuter-dominant usage
- The Olympic period showed decreased cycling activity across the city
- Morning counts strongly correlate with afternoon counts (r=0.81), enabling predictive modeling

## Methodology
Multiple clustering approaches were evaluated:
- K-means clustering with various feature combinations
- HDBSCAN (Hierarchical Density-Based Spatial Clustering of Applications with Noise)
- Log-transformed HDBSCAN to address data skewness

Linear regression was used to predict afternoon traffic based on morning counts, with an R² of 0.786.

## Note on Project Completeness
This repository contains only my contributions to the larger group project. The complete project included additional analyses and model development by my teammates.

## Technologies Used
- Python
- pandas, NumPy
- scikit-learn
- Matplotlib, Seaborn
- HDBSCAN library

---

*This project was completed as part of the DataScientest Data Analyst Bootcamp, September 2024 Cohort.*
