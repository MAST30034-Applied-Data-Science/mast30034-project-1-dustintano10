# MAST30034 Project 1 README.md
- Name: Dustin Edgar Tano
- Student ID: 1188678


Remember, we will be reading through and running your code, so it is in _your best interest_ to ensure it is readable and efficient.

## External Dataset download
This is a guide to download the external dataset/sets. 
1. Nba 2018-2019 attendance dataset
-Go to this link: https://www.basketball-reference.com/leagues/NBA_2019_games.html

-Once in the link see the share and export dropdown and use get table as csv

-Once format changes to csv copy and paste it into an excel file (for the first month, also copy and paste the column names: Date,Start,etc.)

-Do this for the months from October-April (this can be done by just pressing the months and repeating the 2nd and 3rd step)

-Once all is pasted in excel, highlight the only column then go to data, in data press text to column

-In the pop up, press delimited and tick tab and comma as the delimiters, press next and finish

-Save the file with the name nba_attendance_2018_2019 as a csv file

There is also a youtube video to help guide: https://www.youtube.com/watch?v=MWapXbaWs_U&ab_channel=SportsReference
start at the 4:50 min mark 

**Research Goal:** My research goal is Tipping prediction for Yellow Taxi's in relation to the New York Knicks playing

**Timeline:** The timeline for the research area is the 7 months when the nba season runs excluding the playoffs in the years 2018-2019.

To run the pipeline, please visit the `scripts` directory and run the files in order:
1. `script_download.ipynb`: This downloads the raw data into the `data/raw` directory.

To run the files please visit the notebook folder and run the files in order:
1. `preprocess_nba_attendance.ipynb` : This notebook details all preprocessing for the nba_attendance dataset and outputs it to the `data/curated` directory.
2. `preprocess_taxi.ipynb`: This notebook details all preprocessing for the yellow_taxi dataset and outputs it to the `data/curated/yellow` directory.
3. `preprocess_aggregate.ipynb` : This notebook details aggregation for preprocessed taxi data files are outputted in the `data/curated/yellow` directory.
4. `analysis.ipynb`: This notebook is used to conduct analysis on the curated data plots are outputted in the `plots/` directory.
5. `modelling.ipynb`: The ipynb is used to run the model and produce summary statistics these summary statistics are then made into nice tables.
