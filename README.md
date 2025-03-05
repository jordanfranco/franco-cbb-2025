# franco-cbb-2025

The main file is 'NCAAB2025', and the regression output in the first chunk populates the first sheet of the excel file, which should be updated as soon as new games are put in.
Credits to Erik Haslam (https://haslametrics.com/), Ken Pomeroy (https://kenpom.com/), and the team at RealGM (https://basketball.realgm.com/) for their data that supports my analysis. 

This is the earliest stage of this project so the code is pretty humble. I've mainly been using R for the regression output up until this point, so I don't expect this code to wow anyone. The main spreadsheet is far more robust, but I will be putting in some work after March Madness to build this out when I have free time.


The chronology of updating games in the file is pretty straightforward:
1. The day begins. The 'HM', 'KP', and 'RealGM' tabs are updated with current data.
2. The "Template" tab is copied and renamed to match the current day (in the style of Feb 12, Mar 13, Apr 14, etc.). The days matches are input in column F, Away teams are the first row in the pair.
3. Those matchups now populate the corresponding Matchups tab (in the style of Feb12 Matchups, Mar13 Matchups, etc.). It displays the difference in several metrics between the two teams per matchup (negative numbers associated with home-team advantage). It also includes a mechanic of my own creation called 'Aura', which has proven helpful in identifying upsets. It's based in consistency, winning/losing by more/less than you should, win/loss importance, among others.
4. Upon conclusion of a game, record the point differential in the 'Formula Copier' tab, which should be populated by the day's games. After conclusion of all the day's games, copy values and style to 'Reg Model', and copy that into CSV document

There are also lots of resources and fun little tools in there as well. The code will constantly be expanding and growing in complexity, this project will be built upon more over the next several years.