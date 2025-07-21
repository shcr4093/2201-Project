# 2201-Project
This is Shane's project for INFO 2201

This project explores team and individual player performance from major trades from the 2000s to present. Using Python and popular data science libraries, the analysis focuses on how each player perfromed post trade as well as their respecitve teams.

The goal is to tell a data-driven story through clear visuals and well-organized insights that reveal how trades effect franchises

Merging:
The 3 csv's (regular1,2,and 3) were loaded into the file and were merged into one data set for simplicity. This merged dataset is called stats

The "regulartotals" csv contains win loss data that isn't present in the new merged stats dataset. The two data sets will be merged on the season year, game id, and team id columns. The columns names were changed to lowercase so both files are the same for merging

Cleaning:
DeMar DeRozan and Kawhi Leonard

This analysis will explore the points per game and plus minus for each player before and after the trade. Additionally, win percentage and () will be analyszed for each of the teams involved from before and after the trade.

After all the data sets were merged, the new full data set was filtered by setting a variable that contains DeMar DeRozan and Kawhi Leonard.
Afterwards the full data set was aggregated by player and season, calculating total games played, total points scored, and average plus-minus points. Average plus minus and ppg were calculated by standard methods and a new column was created to add the points per game. The charts were created by specifying the time periods that are before and after the trade. Bar charts for indidual changes between the years for the players and teams were provided

