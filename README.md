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
row_id	Unique identifier of a row
scout_id (categorical)	Unique identifier of a scout
winner (categorical)	Player’s team result: winner, loser, or draw
team (categorical)	Team of the player: Team1 or Team2 
team1_system_id (categorical)	Unique Id of Team 1
team2_system_id (categorical)	Unique Id of Team 2
competitionId (categorical)	Competition id of the match
player_position_1 (categorical)	Position 1 of a player in a match
player_position_2 (categorical)	Position 2 of a player in a match
player_height	Transformed height of a player
player_weight	Transformed weight of a player
Player Encoded Variables	Pre encoded variables of a player related to offensive, defensive, positional, physical, general, and other
Team 1 Encoded Variables 	Pre encoded variables of Team 1 related to offensive, defensive and other 
Team 2 Encoded Variables 	Pre encoded variables of Team 2 related to offensive, defensive and other 
rating_num	Rating of a player in a match given by a scout

Variables that encode player properties or performance are grouped according to the following scheme:  
player_(offensive/defensive/positional/physical/general/other)_(derived/raw/ratio)_var_#number
•	player shows if the variable refers to a player property
•	(offensive/defensive/positional/physical/general/other) refers to the nature of the variable
•	(derived/raw/ratio):
o	raw: variable empirically measured
o	derived: variable defined based on two or more variables and not empirically measured
o	ratio: variable defined as a ratio of two raw variables

Variables that encode team properties or performance are grouped according to the following scheme:  
team(1/2)_(offensive/defensive/other)_(derived/raw/ratio)_var_#number
•	team(1/2) shows if the variable refers to a team1 or team2 property
•	(offensive/defensive/other) refers to the nature of the variable
•	(derived/raw/ratio):
o	raw: variable empirically measured
o	derived: variable defined based on two or more variables and not empirically measured
o	ratio: variable defined as a ratio of two raw variables
