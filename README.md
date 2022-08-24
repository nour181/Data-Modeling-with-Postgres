## Project Summary:

##### The objective of this project is to create an analytics database for a music streaming service called Sparkify, they seek to understand what, when and how users are playing songs on the company's music app, they want an easy way to query and analyze data that is on json files on the user activity on their app

#### we will create a star schema database using postgresql and ETL pipelines using python


## Data:

#### the data files contain two datasets:
#### Song datasets and Log datasets

## Database Schema:

#### it's a star shema database contains five table:
##### one fact table that contains all records called(songplays)
##### 4 dimensional table(users, songs, time, artists)

## Data Structure:

#### 1- data folder nested at the home of the project, where all needed jsons reside.
#### 2- sql_queries.py contains all your SQL queries, and is imported into the files bellow.
#### 3- create_tables.py drops and creates tables. You run this file to reset your tables before each time you run your ETL scripts.
#### 4- test.ipynb displays the first few rows of each table to let you check your database.
#### 5- etl.ipynb reads and processes a single file from song_data and log_data and loads the data into your tables.
#### 6- etl.py reads and processes files from song_data and log_data and loads them into your tables.
#### 7- readme file that contains description and details about the project

## Data Processing:

#### Data extracted from from song data file and log data file(json files), json files read into pandas dataframe, processed, and uploaded using psycopg2 into database
#### A number of steps clean the data and reduce the size of the database by removing data not needed for the analysis:

#### Songplays are identified by filtering for actions initiated from the 'NextSong' page.
#### Timestamps are converted from UNIX time to datetime format.

## How to run the project?

#### run create tables and sql_queries from terminal to create tables and execute sql queries, run etl.py to process and load data into database, and in the end run test.ipynb to validate all the past process and execute some sql queries examples
