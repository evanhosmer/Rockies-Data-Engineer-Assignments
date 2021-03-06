# MLB Gameday API Data

This repo contains code to download a days worth of game data from the MLB Gameday API.

## System Dependencies

The script to collect the gameday data for a particular date was written in python 3. To execute this code, python 3+ needs to be utilzed. Some of this code will not execute properly if done using an earlier version of python. The following libraries were used:
- `csv`
- `urllib`

To run this utility:
- Download the files from this repo.
- cd into the Rockies directory.
- Open the `rockies.py` file and edit the input date for the `get_json_grid` and `get_game_data` functions.
- Change the path to the data folder for the output csv to reflect local machine.
- From the command line, type `python rockies.py`
- The csv file will be in the data directory and have a name in the format year-month-day.csv reflecting the input date. 

# 2016 MLB Player Slash Lines

The SQL file to calculate the slash lines for every batter in 2016 is also included in this repo. The file is located in the rockies directory and is named `slash_lines.sql`.

The script calculates the following statistics for each batter in 2016:
- At bats (AB)
- Batting Average (avg)
- On Base Percentage (OBP)
- Slugging Percentage (SLG)
