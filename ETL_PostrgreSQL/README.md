# Schema for Song Play Analysis

Using the song and log datasets, we'll need to create a star schema  optimized for queries on song play analysis. This includes the following tables.

#### Fact Table

1. songplays

    \- records in log data associated with song plays i.e. records with page 

   ```
   NextSong
   ```

   - *songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent*

#### Dimension Tables

1. users

    \- users in the app

   - *user_id, first_name, last_name, gender, level*

2. songs

    \- songs in music database

   - *song_id, title, artist_id, year, duration*

3. artists

    \- artists in music database

   - *artist_id, name, location, latitude, longitude*

4. time

    \- timestamps of records in 

   songplays

    broken down into specific units

   - *start_time, hour, day, week, month, year, weekday*

# Project Template

In addition to the data files, the project workspace includes six files:

1. `test.ipynb` displays the first few rows of each table to let you check your database.

2. `create_tables.py` drops and creates tables. 

3. `etl.ipynb` reads and processes a single file from `song_data` and `log_data` and loads the data into your tables. This notebook contains detailed instructions on the ETL process for each of the tables.

4. `etl.py` reads and processes files from `song_data` and `log_data` and loads them into your tables.

5. `sql_queries.py` contains all your sql queries, and is imported into the last three files above.

   

