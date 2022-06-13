# Football-player-assessment

## Objective
The main goal of the problem is to develop a machine learning algorithm that predicts the scout-made evaluation of players in the context of given matches.


## About Dataset
You are provided the Sevilla FC and FC Bengaluru United large scouting dataset containing the players, teams, and opponent's performance in terms of physical, kinematical, technical, and tactical variables.
Every row of the dataset corresponds to the evaluation of a player in a given match together with variables related to the player, match, team, and opponent and the rating of a player in a match given by a scout.


## Dataset Description
You are provided with 3 files: train.csv, test.csv, and sample_submission.csv. 

## Train and Test set

train.csv and test.csv contain the variables relating to player, match, team, and opponent. The training set includes the target variable rating_num indicating the rating of a player in a match. You need to predict the rating_num in the test set.


## Variable	Description
![image](https://user-images.githubusercontent.com/91201515/173370403-275ab95c-26f1-4dbc-91c5-a5980f2e3f84.png)

Variables that encode player properties or performance are grouped according to the following scheme:  
player_(offensive/defensive/positional/physical/general/other)_(derived/raw/ratio)_var_#number
1.player - shows if the variable refers to a player property
2.(offensive/defensive/positional/physical/general/other) - refers to the nature of the variable
3.(derived/raw/ratio):
         o	raw: variable empirically measured
         o	derived: variable defined based on two or more variables and not empirically measured
         o	ratio: variable defined as a ratio of two raw variables

Variables that encode team properties or performance are grouped according to the following scheme:  
team(1/2)_(offensive/defensive/other)_(derived/raw/ratio)_var_#number
1.	team(1/2) shows if the variable refers to a team1 or team2 property
2.	(offensive/defensive/other) refers to the nature of the variable
3.	(derived/raw/ratio):
                o	raw: variable empirically measured
                o	derived: variable defined based on two or more variables and not empirically measured
                o	ratio: variable defined as a ratio of two raw variables
