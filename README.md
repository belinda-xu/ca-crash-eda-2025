# Exploring Car Collision Patterns in California (2025 YTD)

**Data Source:** [California Crash Reporting System (CCRS)](https://data.ca.gov/dataset/ccrs)

Exploratory Data Analysis (EDA) of California’s 2025 year-to-date crash dataset.

## Tools & Libraries
- **Python** (Pandas, NumPy)  
- **Visualization**: Plotly, Matplotlib  
- **Data**: California Crash Reporting System (CCRS), 2025 YTD  


## Data Cleaning & Preparation
Data Prep:
- Standardized column names and reviewed data types and shape
- Removed columns with >70% missing values and irrelevant fields
- Verified `Collision_id` as a unique identifier
- Checked redundancy between `IsHighwayRelated` and `IsFreeway`
- Handled missing values and ensured dataset integrity


## Exploratory Data Analysis (EDA) and Visualizations
This section explores both **frequency** (how often collisions occur) and **severity** (how many people are injured) across two dimensions: **involved party type** and **collision type**.  
For each dimension, three complementary views are shown:  
- Frequency  
- Severity  
- The relationship between frequency and severity

### Involved Party Analysis
- **Frequency** – Other motor vehicles dominate, followed by fixed objects and parked vehicles.  
![Involved Party Frequency](figures/involved_party_frequency.png)  

- **Severity** – Pedestrian and bicycle crashes have the highest average injuries.  
![Involved Party Severity](figures/involved_party_severity.png)  

- **Frequency vs Severity** – Pedestrian crashes combine **high severity** with **top-5 frequency**.  
![Involved Party Scatter](figures/involved_party_scatter.png)  

### Collision Type Analysis
- **Frequency** – Rear-end is most common, followed by side swipe, hit object, and broadside.  
![Collision Type Frequency](figures/collision_type_frequency.png)  

- **Severity** – Vehicle–pedestrian, broadside, head-on, and overturned are most dangerous.  
![Collision Type Severity](figures/collision_type_severity.png)  

- **Frequency vs Severity** – Broadsides combine **high frequency** and **high severity**, making them especially concerning.  
![Collision Type Scatter](figures/collision_type_scatter.png)  
