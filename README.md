# Space-missions-dashboard
## Power BI Project

<img width="632" alt="Dashboard" src="https://github.com/SaiPravallitha/Space-missions-dashboard/assets/48579534/45353793-3c7d-4959-b3d5-600593377ac3">

---

### Introduction
This is a Power BI project on All Sapce Missions from 1964 to August 2022 called "SPACE MISSION ANALYSIS". This project is to analyze and derive the key insights, which are very interesting for Space Lovers.

Disclaimer: The Dataset, which is used for this project is public domain licenced dataset provided by Maven Analytics.
[https://www.mavenanalytics.io/data-playground?page=2]

---
### Problem Statement
1. How have rocket launches trended across time? Has mission success rate increased?

2. Which countries have had the most successful space missions? Has it always been that way?

3. Which rocket has been used for the most space missions? Is it still active?

---
### Skills Used
The following Power BI features were incorporated.
- Data Extraction
- Data Transformation
- Data Loading
- Dax
- Date Table (New Table)
- Measures
- Data Model
- Report
- Slicers
- Dashboard
- Bookmarks

---
### DAX

Total Mission = COUNT('Space Missions'[Mission])

Total Price = SUM('Space Missions'[Price])

Successful Missions = CALCULATE(COUNT('Space Missions'[Mission]), 'Space Missions'[MissionStatus]="Success")

Failed Missions = CALCULATE(COUNT('Space Missions'[Mission]), 'Space Missions'[MissionStatus] = "Failure")

Success Rate = DIVIDE([Successful Missions], [Total Mission])

Prelaunch Failure = CALCULATE(COUNT('Space Missions'[Mission]), 'Space Missions'[MissionStatus] = "Prelaunch Failure")

Partial Failure = CALCULATE(COUNT('Space Missions'[Mission]), 'Space Missions'[MissionStatus] = "Partial Failure")

---

### SPACE MISSION ANALYSIS Dashboard


---

### Key Insights
- Out of 1265 Missions attempted, 1197 Missions succeed with 94.62% of success rate.
- USA has the most successful missions with 146 missions, and it is followed by France with 81 missions.
- Max. successful active missions done by "CASC" and followed by "SpaceX" companies.
- Most active rocket used for space missions was Falcon 9 Block 5, and Space Shuttle Discovery rocket was used for most retired space missions.
- Overall, nearly 162.3 billion dollars speent for all the space missions.
