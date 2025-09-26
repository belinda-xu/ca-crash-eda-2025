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


## Exploratory Data Analysis (EDA)
This section explores both **frequency** and **severity** of collisions, by involved party type and collision type:

- **Involved Party Analysis**  
  - Most common collision partners: other motor vehicles, pedestrians, bicycles  
  - Pedestrian and bicycle collisions show the highest **average injuries per crash**  
  - Scatterplot highlights trade-offs: common but low-severity vs rare but high-severity events  

- **Collision Type Analysis**  
  - Most frequent: rear-end, sideswipe, hit-object, broadside  
  - Most severe: pedestrian, broadside (T-bone), head-on, overturned  
  - Broadsides combine **high frequency + high severity**, making them a critical target for prevention  
