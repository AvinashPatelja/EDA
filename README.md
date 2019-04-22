# EDA
## IPL Match winner Prediction

![Exploratory_Data_Analysis.png](Exploratory_Data_Analysis.png)

Exploratory Data Analysis refers to the critical process of performing initial investigations on data so as to discover patterns,to spot anomalies,to test hypothesis and to check assumptions with the help of summary statistics and graphical representations.

Predicting the out come of the match, based on the history of the tournament.
Key factors affecting outcomes of matches will be analysed. 
Factors that affect match outcomes could be venue (stadium), city, toss winner, and toss decision (field/bat), batsman, bowler, runs scored, wicket taken etc..

## Description on Data

## Questions answered

How many matches we’ve got in the dataset?
How many seasons we’ve got in the dataset?
Which Team had won by maximum runs?
Which Team had won by maximum wicket?
Which Team had won by closest Margin (minimum runs)?
Which Team had won by minimum wicket?
Which Season had most number of matches?
Which IPL Team is more successful?
Has Toss-winning helped in winning matches?
Toss-winning team opted for Bat/Field - Season wise
Toss-winning team opted for Bat/Field - Team wise
Study on match Result - Normal/Tie/No-result
Result of the match - Team wise

## Packages Required / Profiling

import numpy as np # numerical computing 
import pandas as pd # data processing, CSV file I/O (e.g. pd.read_csv)
import matplotlib.pyplot as plt #visualization
import seaborn as sns #modern visualization
import pandas_profiling

### Dataset / Profiling
 	df_matches = pd.read_csv(r'https://raw.githubusercontent.com/insaid2018/Term-1/master/Data/Projects/matches.csv’)
		profile = pandas_profiling.ProfileReport(df_matches)
		profile.to_file(outputfile="IPL_Match.html")

