# Crash Data Analysis: Road Incidents Uncovered

### Table of Content

- [Project Overiew](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Collection and Data Cleaning](#data-collection-and-data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results and Findings](#results-and-findings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Project Overview

To analyze crash data to identify key factors contributing to road incidents, uncover patterns and high-risk situations, and provide actionable insights that support data-driven road safety strategies and accident prevention measures

![Excel](https://github.com/user-attachments/assets/b147571b-61d6-4c91-9a66-d3e5f5bf4f79)

### Data Source

Car Accident: The primary data set used for this analysis is the "Road Accident Data(AutoRecovered).xlsx", which contains detailed informations about various accidents in the country.

### Tools

- Excel - Data collection and Data Cleaning
- MySQL - Data Analysis
- Excel - Data Visualization, creating reports and Dashboard.
  

### Data Collection and Data Cleaning

In the initial data preparation phase, we performed the following tasks:

  1. Data collection was done using Web Scrapping in Excel
  2. Data loading and inspection.
  3. Handling missing values.
  4. Data cleaning and formatting.

### Exploratory Data Analysis

EDA involved exploring the Road accident data to answer key questions, such as:

  -  The total number of casualties?
  -  The total number of Fatal, serious, and slight casualties?
  -  The total number of casualties by various vehicle types?
  -  The total number of casualties by road surfaces?
  -  The total number of casualties by road type?
  -  Current year casualties Vs Previous year casualties Monthly Trends?
  -  Total casualties by location?
  -  Total casualties by light condition?

### Data Analysis

This was done on MYSQL

This include some functions used to analyze
```MySQL
select count(Accident_Severity) from road_accident_database where Accident_Severity = 'Serious'
```
```MySQL
select count(Vehicle_Type) from road_accident_database where Vehicle_Type = 'Car'
```

###  Results and Findings
1.  The total number of casualties is 417883
2.  Slight casualties make us 84.1% of the total casualties.
3.  There are just 7135 fatal casualties, which is 1.7% of the total casualties.
4.  There were more casualties in 2021, than in 2022.
5.  There are more casualties in the urban areas than in the rural areas.
6.  There are more casualties during the day than at dark.
7.  Dry road surafces have the most accidents in terms of road surfaces.

### Recommendations
1.  Communities needs to be educated on the importances of driving safetly.
2.  Involving local communities, schools, and organizations in road safety initiatives creates a shared responsibility for road safety.
3.  Traffic rules and regulations shoulb be enforced by law enforcement agents.
4.  Provide specialized tranings for drivers.
5.  They Government should invest in Road infrastructure
6.  Ensuring safety for pedestrians and cyclists.
7.  Enforcing speed limits through regular patrolling, speed cameras, and penalties for violations, encourage drivers to adhere to safe speeds, reducing the severity and likelihood of accidents.
8.  Improving the design of intersections plays a pivotal role in minimizing collisions at junctions.
9.  Mandating periodic vehicle inspections is vital to ensure that all vehicles on the road meet safety standards and are roadworthy.

### Limitations
- I had to remove all zero values from age column because they would have affected the accuracy of my conclusions from the analysis.
- Feature Selection
- Data Availability and Quality
- Unobserved Heterogeneity
- Risk Compensation
  



