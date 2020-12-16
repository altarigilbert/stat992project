# Welcome to our stat992project repo!
This is the website containing all materials for the STAT 992 final project from the NFL game prediction team.
- The final report is in stat992_project_report.pdf
- The code for the analysis is in code.R
- The data are in files game.csv and spread_to_odds.csv

# Summary of Work

- Using NFL game data from the 2006 through 2019 seasons, we fit different models to predict NFL game results. 
- For predicting wins or losses, a penalized generalized linear model updated with data every week performs the best among candidate models
- For predicting the point spread, a penalized linear model updated by season performs the best, though not quite good enough to turn a profit 

# Models used

- The Bradley-Terry model to predict the binary outcome variable of a pairwise comparison between teams (which is winning in this context) using the prior season's data as a training set 
- Next, we added an L2 penalty to a generalized linear model with a logit link function, and updated it in two separate ways
- The first method updated the model every season, and the second updated the model every week
- Adding additional covariates to this model does not improve the accuracy
- Next, a similar analysis was performed for the point spread using the same L2 penalty and using a Gaussian (identity) link function

# Summary and Charts

