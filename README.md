# NBA-Injury-Finder
The purpose of this study is to predict injuries in NBA basketball using macro level positioning ( x, y coordinates of the player). Maybe we should be looking at markers of fatigue in general and treat injuries as players in states of heightened fatigue.


Literature Review
Find existing studies on sports injuries, fatigue, etc.
https://pubmed.ncbi.nlm.nih.gov/26439776/
Good article for referencing the validity of our study
What is the Hertz in the data we have?
https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0229212#references
This literature has tables data of Total distance, Acceleration and Deceleration including change of direction (COD), and Average and top speed of elite basketball players.
4.2.1 Total Distance
4.2.2 Accelerations and Decelerations
4.2.3 Average and Top speed
4.2.4 Time motion analysis
https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7206363/
Lower risk of injuries
High weekly distance
Accumulative distance (for season?)
Higher risk of injuries
Low chronic workload
Fatigue (excess total distance)
High distance per minute
Time spent in high-speed zone
Increases in 3-week cumulative distance
rises in 3-week force-load (a cumulative measure of both foot strides and collisions
non-contact soft-tissue injuries have been shown to be associated with increased intensity (Measured in m/min) in the preceding weeks
Acute (1 week) high-speed distance (fatigue) was combined with low chronic (4+ weeks) high-speed distance (fitness)
rapid increases in load increase the risk of injury whereas chronic exposure to higher load strengthens physical capabilities and resilience to injury


Code
Add version control
Data segmentation: to generate a proper set of labeled data, we need condition positives (when injuries occur) and condition negatives (when injuries don’t occur). Condition positives are easy enough to find, but how to select good condition negatives? Can’t just select random clips from the game, because it’s too random.
seconds preceding actual injuries, then find non-injuries that are similar
minutes before actual injuries compared to typical profile for a player
Feature selection: what are some unique things that occur before an injury?
joshua.wrightchisem@gmail.comis thinking up features (sudden lateral accel) that might predict injuries
Could also think of longer term features (player was slowing down significantly before the injury)
Data gathering:
NFL Injury & movement tracking data!
https://www.kaggle.com/c/nfl-playing-surface-analytics/
Data looks very nicely cleaned up
100 non-contact injuries
Movement data 10hz
Movement / sportvu data
https://github.com/linouk23/NBA-Player-Movements/tree/master/data/2016.NBA.Raw.SportVU.Game.Logs
2015-16 season (same set as mine)
find times and players where injuries occur
joshua.wrightchisem@gmail.com is making a spreadsheet of all significant (which injuries did we say count towards this study?) injuries in the 2014-15 and 2015-16 seasons
Existing datasets
https://www.kaggle.com/ghopkins/nba-injuries-2010-2018
https://m.scirp.org/papers/104074
https://www.prosportstransactions.com/basketball/
https://www.mangameslost.com/ (2014 -2016 seasons but need to pay for access)
Covid19 - json dataset
https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge
Dense data with all json files
Uses algos like TSN-E to analyze
What exactly do we count as an injury?
Lower extremity with rest of game missed



