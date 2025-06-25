# Neighbourhood Crime Insights (NCI)

**A Machine Learning-Based Crime Clustering and Analysis System for Nova Scotia**

## Overview

Neighbourhood Crime Insights (NCI) is a data-driven project that explores the spatial and socio-economic patterns of crime in Nova Scotia. Using unsupervised clustering techniques, particularly HDBSCAN, this system analyzes over 24,000 records of crime reports combined with demographic data from the 2016 and 2021 Canada Census to detect high-risk regions and derive community-level insights.

This project was developed as part of the *CSCI6409: Process of Data Science* course at Dalhousie University.

## Key Features

- **Spatio-Socioeconomic Crime Clustering**  
  Utilizes HDBSCAN to uncover meaningful crime clusters across urban and rural communities, identifying noise/outlier zones for further investigation.

- **Multi-Year Analysis**  
  Integrates data from both 2016 and 2021 to track shifts in crime patterns and socio-economic conditions over time.

- **Feature Engineering**  
  Combines normalized crime rates with demographic indicators such as income, education, age group distributions, and minority status.

- **Interactive Visualizations**  
  Uses Folium maps and scatter plots to validate clusters and present crime zones with contextual socio-economic overlays.

- **Scalable Methodology**  
  Designed for future extension to real-time monitoring systems or comparative studies across Canadian provinces.

## Methodology

1. **Data Sources**  
   - Nova Scotia Open Crime Data  
   - Canada Census (2016 & 2021)

2. **Preprocessing Pipeline**  
   - Handled missing values, normalized crime rates per 100,000 population  
   - One-hot encoded categorical features and standardized numerical features  
   - Merged datasets based on geographic identifiers

3. **Clustering Algorithms**  
   - K-Means and DBSCAN were tested, but HDBSCAN was selected for its robustness in handling clusters of varying density  
   - Achieved a Silhouette Score of **0.87**, indicating high-quality clustering performance

4. **Cluster Insights**  
   - High-crime clusters correlated with low income, aging populations, and limited education (e.g., Cape Breton, Annapolis Royal)  
   - Low-crime clusters exhibited higher post-secondary education and stronger economic indicators (e.g., Amherst, Enfield)  
   - Outlier cluster (Cluster -1) indicated regions undergoing transitional dynamics or exhibiting mixed traits

## Tech Stack

- **Languages:** Python  
- **Libraries:** Pandas, NumPy, scikit-learn, HDBSCAN, Matplotlib, Seaborn, Folium  
- **Tools:** Jupyter Notebooks, Git, GitHub  
- **Data Sources:** Nova Scotia Open Data Portal, Statistics Canada

## Results

- Identified 21 distinct clusters across Nova Scotia with differentiated crime and socio-economic profiles
- Demonstrated a decline in average crime rates between 2016 and 2021 in parallel with an increase in median income
- Highlighted the importance of education and community resilience in mitigating crime risk

## Future Work

- Expand to include real-time data feeds (e.g., 911 call records)
- Build an interactive dashboard for stakeholders (e.g., policymakers, municipalities)
- Incorporate explainable AI methods (e.g., SHAP) for better model interpretability
- Generalize the approach to other provinces for nationwide comparative studies

## Authors

- **Viren Joshi**
- **Samruddhi Mulay**  
- **Shreya Rao**

This project is intended for academic and research purposes.
