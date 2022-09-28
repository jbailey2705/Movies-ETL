# Movies-ETL

## Project Overview

Amazing Prime loves the dataset and wants to keep it updated on a daily basis. Within the scope of the Amazing Prime Hackathon, for this profject we will be required to create an automated pipeline that takes in new data from Wikipedia data, Kaggle metadata, and MovieLens rating data. We'll perform the appropriate transformation and load the data into SQL Postgre database.

For this we'll use the following:

1. write an ETL function to read 3 data files
2. extract & transform the Wikipedia data
3. extract & transform the Kaggle and rating data
4. load the data to a PostSQL data base called "movie_data"

## Resources:
- Data Sources: [wikipedia-movies.json.zip](https://github.com/jbailey2705/Movies-ETL/files/9668534/wikipedia-movies.json.zip), [movies_metadata.csv.zip](https://github.com/jbailey2705/Movies-ETL/files/9668536/movies_metadata.csv.zip), [ratings.csv](https://github.com/jbailey2705/Movies-ETL/files/9668631/ratings.csv)
- Software: Python 3.7.7, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3, PostgreSQL 11.9, pgAdmin 4

## Results with detail analysis:

### Write an ETL fuction to read 3 data files
Funciton takes Wikipedia JSON, Kaggle metadata, & MovieLens csv files to create three DataFrames.

### Extract and Transform the Wikipedia data
We've filtered out TV shows, consolidated the redundant data, removed duplicates & formated the Wiki data.

### Extract and Transform the Kaggle and rating data
Consolidated redundant data, removed any duplicates, grouped & formatted the data. Kaggle & rating data were merged with the Wiki movies DataFrame

<img width="667" alt="Ratings_updated" src="https://user-images.githubusercontent.com/109354592/192901516-0c621388-1087-49fb-b5fd-02e06dbda7c0.png">
![Scree<img width="663" alt="Movies_updated" src="https://user-images.githubusercontent.com/109354592/192901527-50e99cb6-0fd4-4e52-84e0-f79ac189b4e7.png"

<img width="663" alt="Movies_updated" src="https://user-images.githubusercontent.com/109354592/192901554-89703f2f-3bb8-4ec4-9184-0a2723ba0c63.png">
![Screen Shot 2022-09-28 at 5 31 45 PM](https://user-images.githubusercontent.com/109354592/192900145-a9302691-8d86-4631-8234-fdfb06f1cb80.png)

## Summary
The ETL function collects & cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). The function transforms & merges  data, loads it into two updatable PostgreSQL dataset tables (provided) ready to be used by the hackathon participants for analysis.

