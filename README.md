# PKL-2019-Predictions

**For TASK 1 and TASK 2:**

Task 1: Predict the winner of the tournament.
Task 2: Predict the top team in the points table after the completion of the league matches.

NOTE:- TASK 2 done before TASK 1, since League matches complete first and then final winner is predicted.

APPROACH:

Data was extracted from the site https://www.prokabaddi.com/ using Selenium and BeautifulSoup.
Data was extracted for the various matches played in Season 7 and Season 6, along with the scores of each game and the winner of each game.

Data was extracted for the current Standings of the Teams in the League table.
Data was extracted for the matches pending of the current season. (Season 7).

Data was analysed and prepared for modelling to predict the outcome of pending matches using the historical data of matches.

A logistic Regression Model was made for this purpose.
An accuracy of 66.66% was observed on the train set and 63.5% was observed on Test Set.

So, given a pair of teams this Model would give us which team is likely to be the winner.
A function was created to simulate this.

Predictions were made on All Pending Matches of the current Season and the Standings table was accordingly updated.

Based on the final Predicted League Table Standings, we observed that "BENGAL WARRIORS" are on top and thus would be the Winner of League Stage.

**ANSWER TASK 2: BENGAL WARRIORS WOULD WIN LEAGUE STAGE**

The TOP-6 teams were taken to be qualified. The top-2 were in semi-finals and other 4 had to undergo Eliminator Matches.
Again Simulations were Made for these matches to Predict the winner.
Based on the prediction outcomes the Semi-finalists were predicted.
And again prediction output on those semi-final and final matches, it was Predicted that "BENGAL WARRIORS" would WIN the FINAL MATCH.

**ANSWER TASK 1: BENGAL WARRIORS WOULD WIN TOURNAMENT**


**TASK 3 and 4**

Task 3: Predict the team with the highest points for successful raids.
Task 4: Predict the team with the highest points for successful tackles

APPROACH:
Task 3 and 4 had similar approach and hence described together.

Data was extracted from the site https://www.prokabaddi.com/ using Selenium and BeautifulSoup.
Data was extracted for the various Teams, their matches played and RAID points in Season 7, Season 6 and ALL SEASONS COMBINED. 
Data was extracted for the various Teams, their matches played and TACKLE points in Season 7, Season 6 and ALL SEASONS COMBINED.

DATA was analysed and various metrics were generated such as,
Avg Raid Points for Season 7
Avg Raid Points for Season 6
Avg Raid Points for All Seasons Combined,
Percentage Change in AVG Raid Points of Season 7 as compared to Avg of Season 6.
Percentage Change in AVG Raid Points of Season 7 as compared to Avg of All Seasons combined.

For Task 4, metrics generated were
Avg Tackle Points for Season 7
Avg Tackle Points for Season 6
Avg Tackle Points for All Seasons Combined,
Percentage Change in AVG Tackle Points of Season 7 as compared to Avg of Season 6.
Percentage Change in AVG Tackle Points of Season 7 as compared to Avg of All Seasons combined.

Using these metrics and historical data, A simple Linear Regression Model was Built to predict the Average Raid Points and Average Tackle Points for Season 7 of the Top Teams.
Model was evaluated on the Mean Squared Error using K-fold Cross Validation.

Using this, the final Total Successful Raid Points and Total Successful Tackle Points were Predicted for the teams.
Therefore,

**ANSWER TASK 3: DABANG DELHI K.C. WOULD have highest points for successful RAIDS**
**ANSWER TASK 4: PUNERI PALTAN  WOULD have highest points for successful TACKLES**


**TASK 5: Predict the team with the highest super-performance total.**

APPROACH:
Approach of Task 3 and 4 was Extrapolated for Task 5.

Data was extracted from the site https://www.prokabaddi.com/ using Selenium and BeautifulSoup.
Data was extracted for the various Teams, their matches played and the following Data
Super Raids
Super Tackles
All-Outs Inflicted
All-Outs Conceded

DATA was analysed and various metrics were generated such as,
Avg SPT for Season 7
Avg SPT for Season 6
Avg SPT for all Seasons Combined

Using these metrics and historical data, A Linear Regression Model was made to predict the Avg SPT of Teams.
Model was evaluated on the Mean Squared Error using K-fold Cross Validation.

**Answer of TASK 5: BENGAL WARRIORS would have the highest super-performance total.**

**TASK 6 and 7**

Task 6: Predict the player with the highest SUCCESSFUL RAID percentage.
Task 7: Predict the player with the highest SUCCESSFUL TACKLE percentage.

APPROACH:
Task 6 and 7 had similar approach and hence described together.

Data was extracted from the site https://www.sportskeeda.com/go/pro-kabaddi/successful-raids-percentage-player 
and https://www.sportskeeda.com/go/pro-kabaddi/successful-tackles-percentage-player
using Selenium and BeautifulSoup.

On analysing the Data it was observed that the percentage point gap between highest and second highest was extremely wide and that the remaining number of matches for that team would not be sufficient to cross-over, and thus,

**ANSWER TASK 6: SAURABH NANDAL WOULD have the highest SUCCESSFUL RAID percentage.**
**ANSWER TASK 7: Ravindra Ramesh Kumawat  WOULD have the highest SUCCESSFUL TACKLE percentage.**

# THE END
