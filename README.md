# 2201-Project
This is Shane's project for INFO 2201

This project analyzes the short-term and long-term effects of two major NBA trades:
1. **DeMar DeRozan ↔ Kawhi Leonard (2018)**
2. **Shai Gilgeous-Alexander ↔ Paul George (2019)**

##  **Objective**
Using Python and popular data science libraries, the analysis focuses on how each player perfromed post trade as well as their respecitve teams.
The goal is to tell a data-driven story through clear visuals and well-organized insights that reveal how trades effect franchises

##  **Data Sources**
**Link To Source**
https://github.com/NocturneBear/NBA-Data-2010-2024?tab=readme-ov-file

The data used is found in this github repository. It contains 3 csv files with compregneisve NBA data that covers 2010-2014 at the individual level. It provides many useful and unique performance metrics for player. Some metrics included are points scored, minutes, free throw percentage, three point percentage, assists, steals, plus minus, blocks, etc. Thee 4th csv file contains the same dimensions but aggregated per team.

##  **Merging**
The 3 csv's (regular1,2,and 3) were loaded into the file and were merged into one data set for simplicity. This merged dataset is called stats
The "regulartotals" csv contains win loss data that isn't present in the new merged stats dataset. The two data sets will be merged on the season year, game id, and team id columns. The columns names were changed to lowercase so both files are the same for merging

##  **Cleaning**
**DeMar DeRozan ↔ Kawhi Leonard (2018)**

This analysis will explore the points per game and plus minus for each player before and after the trade. Additionally, win percentage and () will be analyszed for each of the teams involved from before and after the trade.

After all the data sets were merged, the new full data set was filtered by setting a variable that contains DeMar DeRozan and Kawhi Leonard.
Afterwards the full data set was aggregated by player and season, calculating total games played, total points scored, and average plus-minus points. Average plus minus and ppg were calculated by standard methods and a new column was created to add the points per game. The charts were created by setting keys to find information in the data set. The keys used would be the player names and the years before and after the trade. After the keys were set, they were essentially used as a lookup step to find all relevant information on those 2 players. Next the relevant data was referenced (points scored and plus minus) and then the data was plotted into a chart comparing the 2 years for each player. For the team performance, the keys used for the team charts were the abbreviated team names (Toronto / TOR) and years before and after the trade. The code .drop duplicates was used otherwise each player on a teams roster would contribute a W per real team win. There should only be 82 games total for each team. After the data was filtered, both charts were created.

**Shai Gilgeous-Alexander ↔ Paul George (2019)**
The same process above was used to filter and create the visualizations for this trade

##  **Visualizations**
**DeMar DeRozan ↔ Kawhi Leonard (2018)**
The average plus minus data before and after the trade highlights a more significant insight. Both Kawhi Leonard and DeMar DeRozan saw a noticeable decline in their average plus-minus after the trade. For Kawhi, the decline was moderate, but DeRozan’s drop was substantial. This implies that while DeRozan maintained or even improved his scoring output, his on court impact on team success was diminished in San Antonio compared to Toronto. It shows that high individual scoring doesn’t always equate to better team performance

**Shai Gilgeous-Alexander ↔ Paul George (2019)**
The plus minus trends following the trade between the Clippers and Thunder reveal a deeper narrative beyond surface level stats. Shai Gilgeous-Alexander, initially viewed as a developing young guard, showed significant growth in his impact on team performance after moving to Oklahoma City. His shift from a slightly negative plus-minus to a clearly positive one suggests he not only adapted but thrived in a larger role. Paul George experienced a slight decline in plus minus despite remaining a high level performer in Los Angeles. This may reflect the challenges of fitting into a superstar duo system alongside another dominant player, or the pressure of playing for a contender with championship expectations.

**Teams Win Loss**
The Toronto Raptors saw a -1.69% decrease in wins during the season following the trade with San Antonio. The San Antonia Spurs saw a +2.13% increase in wins following the same trade. 
The Okloahom City Thunder saw a -10.2% decrease in wins during the season folliwing the trade with Los Angeles. The Los Angeles Clippers saw a +2.1% incrase in wins following the same trade.

##  **Insight**
The DeRozan Kawhi trade showed that while both players continued to be productive scorers, their overall impact on team success shifted. Kawhi helped Toronto reach a championship level, while DeRozan’s influence on wins declined despite similar or better scoring numbers.

Shai Gilgeous-Alexander’s role and value grew significantly after being traded to OKC. His impact on winning became much more noticeable, showing that the trade gave him the space to develop into a franchise player. Paul George remained effective but had a slightly reduced impact in a new system with another star player.

Team win-loss records suggest that short-term team performance doesn’t always change drastically after a blockbuster trade. San Antonio slightly improved and Toronto slightly declined after the trade, but neither change was dramatic. The OKC-LAC trade had a clearer effect, with OKC declining in wins and the Clippers improving slightly, likely due to a win-now focus.

Overall, the impact of trades goes beyond scoring. Player roles, team fit, and long-term development are key to understanding the real effects of high-profile moves.
