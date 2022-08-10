# MAST30034 Project 1 README.md
- Name: Dustin Edgar Tano
- Student ID: 1188678

## Student Instructions
You **must** write up `README.md` for this repository to be eligable for readability marks.

1. Students must keep all Jupyter Notebooks in the `notebooks` directory.
2. Students must keep all `.py` scripts under the `scripts` directory. These can include helper functions and modules with relevant `__init__.py`
3. Students must store all raw data downloaded (using a Python script) in the `data/raw` folder. This will be in the `.gitignore` so **do not upload any raw data files whatsoever**.
4. Students must store all curated / transformed data in the `data/curated` folder. This will be in the `.gitignore` so **do not upload any raw data files whatsoever**. We will be running your code from the `scripts` directory to regenerated these.
5. All plots must be saved in the `plots` directory.
6. Finally, your report `.tex` files must be inside the `report` directory. If you are using overleaf, you can download the `.zip` and extract it into this folder.
7. Add your name and Student ID to the fields above.
8. Add your relevant `requirements.txt` to the root directory. If you are unsure, run `pip3 list --format=freeze > requirements.txt` (or alternative) and copy the output to the repository.
9. You may delete all `.gitkeep` files if you really want to. These were used to ensure empty directories could be pushed to `git`.
10. When you have read this, delete the `Student Instructions` section to clean the readme up.

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

**Research Goal:** My research goal is Does New York Knicks games have any influence on taxi profits and area popularity?

**Timeline:** The timeline for the research area is 2018 - 2019.

To run the pipeline, please visit the `scripts` directory and run the files in order:
1. `script_download.ipynb`: This downloads the raw data into the `data/raw` directory.
2. `preprocess.ipynb`: This notebook details all preprocessing steps and outputs it to the `data/curated` directory.
3. `analysis.ipynb`: This notebook is used to conduct analysis on the curated data.
4. `model.py` and `model_analysis.ipynb`: The script is used to run the model from CLI and the notebook is used for analysing and discussing the model.
