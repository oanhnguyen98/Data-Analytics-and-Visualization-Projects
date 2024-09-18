# Civil Aviation Accidents - Tableau Data Visualization Project 

# Project Overview
This project focuses on analyzing trends in aviation accidents using data from the Aviation Accident Database & Synopses up to 2023, sourced from the National Transportation Safety Board (NTSB). The aim is to uncover insights into the causes and severity of aviation accidents, with a focus on improving the safety and quality of air travel. The project employs a variety of visualizations to explore the number of accidents, injuries, fatalities, and accident causes over time, as well as correlations between weather conditions, flight purposes, and accident severity.

The key business questions addressed in the project include:

- What are the most common phases of flight where accidents occur?
- How does weather impact accident rates and severity?
- What types of aircraft and engines are most involved in accidents?
- What are the trends in accident-related injuries and fatalities over time?

![Data Visualization Poster](images/Data%20Visualization%20Poster.jpg)

The final visualizations are published on Tableau Public and can be accessed [here](https://public.tableau.com/app/profile/ngoc.oanh.nguyen/viz/Nguyen_NgocOanh_DataVisualizationProject/Story_CivilAviationAccidents).

# 1. Dataset Information
The [dataset](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses?datasetId=521&sortBy=voteCount) used for this project, AviationData.csv, is sourced from Kaggle and contains data on civil aviation accidents and selected incidents from 1962 to 2023. The dataset includes:

- Accident Information: Date, location, phase of flight, weather conditions.
- Injuries: Total injuries, including breakdowns of fatal, serious, minor, and uninjured cases.
- Aircraft Information: Aircraft category, engine type, and damage severity.
- Flight Purpose: Categories like personal, business, or commercial flights.
The dataset is relatively clean, but some missing values and non-visualizable attributes were filtered out before creating visualizations.

# 2. Data Preparation:
- Removed non-visualizable attributes like Report.Status and Registration.Number.
- Filtered missing values from important fields like Event.Date and Publication.Date.
- Focused on injury counts and severity as key measures due to the dataset’s limitations in numeric attributes.

# 3. Key Visualizations & Analysis

3.1. Accident Trends Over Time:

- Line Charts with Motion: Shows the change in total injuries over time, with motion to animate trends.
- Insights: Reciprocating engines are involved in the most accidents, though this may correlate with their common usage rather than inherent issues.

3.2. Injury Severity:

- Stacked Bar Chart: Visualizes the severity of injuries (fatal, serious, minor) alongside aircraft damage type.
- Insights: Aircraft destruction correlates with the highest number of fatalities, emphasizing the serious consequences of major accidents.

3.3. Accidents by Flight Phase:

- Bar Chart: Highlights the phases of flight where most injuries occur (e.g., takeoff, maneuvering, cruise).
- Insights: Many injuries occur during takeoff and maneuvering, suggesting these are critical phases for flight safety improvements.

3.4. Geographical Distribution:

- Map: Shows the distribution of injuries across different countries.
- Insights: The U.S. accounts for the majority of accidents, but the dataset is biased toward U.S. data, limiting international comparisons.

3.5. Weather vs. Flight Purpose:

- Bubble Chart: Analyzes the correlation between weather conditions and the purpose of flights in relation to accident severity.
- Insights: Most accidents occur under favorable weather conditions (VMC) and are related to personal flights, indicating that human factors may be more important than weather in many cases.

3.6. Aircraft & Engine Type:
- Pie Charts: Show the proportion of accidents by aircraft category and engine type.
- Insights: Airplanes and helicopters are the most common categories involved in accidents, with reciprocating engines being the most prevalent engine type.

# Conclusion
This project provided valuable insights into aviation accidents, emphasizing critical phases of flight and the importance of injury prevention. The visualizations offer actionable data for aviation professionals to improve safety measures. While the dataset’s limitations affected the depth of analysis, the project demonstrated the effectiveness of using data visualization to explore complex accident data.
