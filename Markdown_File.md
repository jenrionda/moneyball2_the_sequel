Moneyball 2: The Sequal

By Jennifer Rionda, George Smith, Zach Steindam

![mlb_pic](\mlb_pic.jpg)

Legal sports betting is a $5B per year revenue market that is expeceted to grow upwards of $7B by 2025. By 2021 sports betting is expected to be legal in 36 states. 

To capitalize on this market we have decided to build a MLB machine learning model to predict the outcomes of any given matchup between two teams. 

We chose baseball because of the very large data set that is publicly available, which we thought would be perfect for a machine learning model!

We got our data from retrosheet.org, which has the box scores for each game going back to 1871 publicly available and organized into very nice excel files.
We took running and rolling averages of certain stats that we thought would be important to help model matchup winners.

![retro_logo](\retro-logo.gif)


We also got some great data from FiveThirtyEight. The curated a data ELO Dataset, which created a running team ranking as well as a running pitcher ranking.

We concated these two data frames and ran them into a few models. The industry standard for these types of models is XGBoost. We found that this gave us our best accuracy score at 58.2%. Below are the top features from out XGBoost model.

![top_ten_features](\top_ten_features.png)

Benchmarked against a Vegas score of 56.7% we are about 1.5% ahead!
