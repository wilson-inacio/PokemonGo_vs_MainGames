# The Impact of Mainline Pokémon Game Releases on Pokémon GO Player Activity
## Introduction
This project investigates whether the release of mainline Pokémon games has had a measurable impact on player activity in Pokémon GO. The central hypothesis is that the release of a new core Pokémon title is associated with an increase in Pokémon GO player activity, potentially due to renewed interest in the franchise.

To evaluate this hypothesis, two datasets are used: one containing estimated monthly Pokémon GO player activity since the game’s launch, and another listing the release dates of mainline Pokémon games. By comparing trends in player activity with the timing of game releases, this analysis aims to identify potential patterns or correlations between the two. We’ll also do some linear regression to identify what is the relation between the release of new games and Pokémon Go activity, and make some basic predictions for 2026.

###### Notes:
###### * For the purposes of this analysis, “mainline Pokémon games” refers to core series releases on Nintendo platforms, including the Pokémon: Let’s Go and Pokémon: Legends series. Spin-off titles such as Pokémon Mystery Dungeon, Pokémon Sleep, and Pokémon UNITE are excluded.
###### * Niantic does not publicly disclose detailed player activity metrics for Pokémon GO. As a result, the dataset containing estimated monthly player activity was compiled from multiple third-party sources, including Statista, Active Player, and Business of Apps. These figures represent approximations rather than exact values; however, they are considered sufficient for identifying high-level trends relevant to this project.



## Data
On our project we used two csv files, estimated_go_players_monthly.csv containing data on the MAU (Monthly Active Users) estimation since the launch of Pokémon GO, and pokemon_games_release_dates.csv containing the dates with the release dates of the Nintendo platform games.

## Analysis
After some data wrangling with the aim of optimizing the datasets for the project, some exploratory data analysis was conducted to better understand the data.
We gathered insight into the Monthly Active Users (MAU) of Pokémon GO since its inception, and cross-referenced it against the release of mainline Pokémon games. Then, Google Trends was used ot gather insight into Google searches with the term "Pokémon GO" on them and it they had any correlation with mainline game releases.
Linear regression was then used to fit three models: model 1 does linear regression on the release window only, model 2 does a linear regression while taking into account the time trend, and model 3 looks into games post-release effects in Pokémon GO.
Finally, another linear regression model was used to try to predict MAU for each quarter of 2026.

## Conclusion and Further Work
At the start of this project, my assumption was that whenever a new Pokémon game came out, there would be a slight spike in Pokémon Go player activity, as this would regenerate interest in the franchise, but the analysis conducted with this project actually reflects the opposite: That player engagement tends to have a dip during and shortly after a new game comes out, and from here, one can extrapolate that it’s actually the new games that temporarily take attention away from Pokémon Go. We also make the discovery that in the last couple of years, not only has the Pokémon Go game seen an increase and then stabilizing of its player base, but the trend observed actually flipped, with Pokémon Go seing a small increase shortly after a new mainline game comes out. We could also confirm that the release of new games has little to no effect in google searches for Pokémon Go. With the data that we have available to us, it was possible to make some predictions for 2026, that would put the MAU (Monthly Active Users) close to 95 Million users for each trimester.

Going forward, it would be ideal to conduct this reasearch with official numbers released by Niantic, and some other Pokemon related queries in Google trends.
