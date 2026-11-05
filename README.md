# BBL Win Probability Model

A ball-by-ball win probability model for Big Bash League run chases, built from raw Cricsheet data with logistic regression. It asks which factors have the biggest influence on whether a chasing team wins.

## What it does

1. Imports ball-by-ball data, which includes each delivery in the BBL. 
2. Builds features for each ball of a second innings: runs required, required run rate, wickets lost, runs in the last six legal balls, wickets lost in the last 2 overs and Elo difference between the two teams.
3. Trains a logistic regression on the oldest 80% of matches and tests it on the newest 20%.
4. Plots win probability through some of the BBL's most memorable chases.

## How to run
**Locally:**

```bash
git clone https://github.com/rajkulkarni8/bbl_win_probability_model.git
cd bbl_win_probability_model
pip install -r requirements.txt
```
Then open `bbl_chase_analysis_final.ipynb` in VS Code or Jupyter and run all cells. Tested on Python 3.15

## Data

Match data from [Cricsheet](https://cricsheet.org). Cricsheet updates its files, so results may differ slightly with newer data.
Data was sourced from Cricsheet and parsed then converted to a .csv file. 

## Notes

Parts of this project were developed with the help of AI tools.


## Author

Raj Kulkarni