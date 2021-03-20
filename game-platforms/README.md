# Analysis of promising games

## Description:

The dataset consists of historical regional sales of games by platforms, ratings, genre, and scores

**Purposes**: 
- determine the most promising platforms
- model a typical user portrait
- check 2 hypotheses about user ratings

**Features**:
- `Name` — name of a game
- `Platform` — name of a platform
- `Year_of_Release` — year of game release
- `Genre` — game genre
- `NA_sales` — sales in the North America (mn copies sold)
- `EU_sales` — sales in  Europe (mn copies sold)
- `JP_sales` — sales in Japan (mn copies sold)
- `Other_sales` — sales in other countries (mn copies sold)
- `Critic_Score` — critic score (max 100)
- `User_Score` — user score (max 10)
- `Rating` — maturity rating issued by ESRB (Entertainment Software Rating Board)

## Tools used:
- for tables - `pandas`
- for visualization - `seaborn`, `matplotlib.pyplot`
- for hypotheses testing - `scipy.stats`

## Results:
- Popularity of platforms, genres and maturity ratings depend on the market a lot as Japanese customers have specific preferences as of 2017
- In general, PS4 and XOne seemed to be the most promising platforms
- The most popular genres as of 2017 were Action, Shooter, Role-playing and Sports
- Games for everybody and maturity games were of high popularity
- While critic scores had some positive influence on sales, user scores do not
- There is no statistical evidence about differences in user scores of PC and XOne  while user score of Action and Sports differed
