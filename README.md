# MLB -- Modeling the Importance of the 3 Phases to Wins
In this project, we use three OLS models to estimate the importance of an MLB team's pitching, fielding, and batting performance during a season to their Win%.
 
## Data
Our data includes basic batting statistics like HR, H, and OPS+. Pitching stats including SO, FIP, and WHIP can also be found in the data. Some fielding stats in the data include DefEff, E, and Fld%. 

*The data for this project was courtesy of BaseballReference.*
*Link: https://www.baseball-reference.com/*

## Code -- Web Scraping
`MLBFinalProject.ipynb`
Includes code to scrape every team's basic batting, pitching, and fielding data from BaseballReference. We also scrape the standings for each season from 2000-2019 and join that data with the team stats for those years.

## Code -- Creating the Visualizations
`VisualizationsCode.ipynb`
Includes code to create our four visualizations used in our presentation. Three of the visuals are boxplots summarizing team performance in terms of R/G (Batting), RA/G (Pitching), and DefEff (Fielding). The fourth visualization is a correlation plot showing the relationships between Win% and some of the variables we include in our models.

## Code -- Implementing the Models
`FinalProjectModels.ipynb`
Includes code to implement the three models used in our presentation. The first model regresses RS (Batting) and RA (Pitching/Fielding) to Win%. The second regresses different batting stats to RS and the third model regresses different pitching and fielding stats to RA.