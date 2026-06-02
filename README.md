# Who Vanished on the Spaceship Titanic? 

The Spaceship Titanic hit a hidden anomaly in space, and nearly half its
8,693 passengers were swept into another dimension. This project answers one
question: **could we have predicted who?**

**Result: 0.80 accuracy on the Kaggle leaderboard (top ~25–30%).**

## The biggest clue
Passengers asleep in CryoSleep were transported **81%** of the time, versus
just **33%** of those awake. Spending told the same story: people who spent
nothing usually vanished (because frozen passengers can't shop).

## What I did
- Cleaned missing data with logic, not guesswork (e.g. deduced CryoSleep from spending)
- Built new clues: travel group, group size, cabin deck and side, total spending
- Compared models from a simple baseline up to gradient boosting
- Validated honestly with 5-fold cross-validation (my test score matched the real Kaggle score)

## Tech
Python · pandas · scikit-learn · LightGBM · matplotlib

## The lesson
The best insight isn't the fanciest model. It's finding the one clue that
explains the most, and telling that story clearly.
