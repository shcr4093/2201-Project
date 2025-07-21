# 2201-Project
This is Shane's project for INFO 2201

This project analyzes the short-term and long-term effects of two major NBA trades:
1. **DeMar DeRozan ↔ Kawhi Leonard (2018)**
2. **Shai Gilgeous-Alexander ↔ Paul George (2019)**

##  **OBJECTIVE**
Using Python and popular data science libraries, the analysis focuses on how each player perfromed post trade as well as their respecitve teams.
The goal is to tell a data-driven story through clear visuals and well-organized insights that reveal how trades effect franchises

##  **Data Sources**
For this project, the data sets that will be used are from Kaggle. There are 4 total data pieces, all of which are csv files. Three of the files are individual player stats for specific game ids throughout 2010-2024. Some metrics included are points scored, plus minus, rebounds, shots taken, 3 point percentage, etc. The fourth data piece includes the same unique game ids except this one contains stats for the teams themselves instead of the individual level. This analysis will look specifically at performance metrics (ppg, plus minus, win percentage) to understand how the trades effected each team.

##  **Merging**
The 3 csv's (regular1,2,and 3) were loaded into the file and were merged into one data set for simplicity. This merged dataset is called stats
The "regulartotals" csv contains win loss data that isn't present in the new merged stats dataset. The two data sets will be merged on the season year, game id, and team id columns. The columns names were changed to lowercase so both files are the same for merging

##  **Cleaning**
**DeMar DeRozan ↔ Kawhi Leonard (2018)**

This analysis will explore the points per game and plus minus for each player before and after the trade. Additionally, win percentage and () will be analyszed for each of the teams involved from before and after the trade.

After all the data sets were merged, the new full data set was filtered by setting a variable that contains DeMar DeRozan and Kawhi Leonard.
Afterwards the full data set was aggregated by player and season, calculating total games played, total points scored, and average plus-minus points. Average plus minus and ppg were calculated by standard methods and a new column was created to add the points per game. The charts were created by specifying the time periods that are before and after the trade. After all new data is collected the chart for each player was made. For the team performance, the year , team tri code (LAL, SAS, OKC, etc) and other relvant stats were filtered. .drop duplicates was used otherwise each player on a teams roster would contribute a W per real team win. There should only be 82 games total for each team. After the data was filtered, both charts were created.

**Shai Gilgeous-Alexander ↔ Paul George (2019)**

This analysis will explore the points per game and plus minus for each player before and after the trade. Additionally, win percentage and () will be analyszed for each of the teams involved from before and after the trade.
