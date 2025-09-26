# Exploring Car Collision Patterns in California (2025 YTD)
Exploratory Data Analysis (EDA) of California’s 2025 year-to-date crash dataset from the [California Crash Reporting System (CCRS)](https://data.ca.gov/dataset/ccrs).  
The goal is to identify **patterns in collision frequency and severity**, focusing on involved parties (e.g., pedestrians, vehicles) and collision types (e.g., rear-end, broadside).  


## Tools & Libraries
- **Python** (Pandas, NumPy)  
- **Visualization**: Plotly, Matplotlib  
- **Data**: California Crash Reporting System (CCRS), 2025 YTD  


## Data Cleaning & Preparation
Steps taken to prepare the dataset:
- Standardized column names and inspected data types
- Removed columns with >70% missing values and irrelevant fields
- Verified `Collision_id` as a unique identifier
- Checked redundancy between `IsHighwayRelated` and `IsFreeway`
- Handled missing values and ensured dataset integrity


## Exploratory Data Analysis (EDA)
This section explores both **frequency** and **severity** of collisions:

- **Involved Party Analysis**  
  - Most common collision partners: other motor vehicles, pedestrians, bicycles  
  - Pedestrian and bicycle collisions show the highest **average injuries per crash**  
  - Scatterplot highlights trade-offs: common but low-severity vs rare but high-severity events  

- **Collision Type Analysis**  
  - Most frequent: rear-end, sideswipe, hit-object, broadside  
  - Most severe: pedestrian, broadside (T-bone), head-on, overturned  
  - Broadsides combine **high frequency + high severity**, making them a critical target for prevention  
