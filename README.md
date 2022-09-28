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

![Screen Shot 2022-09-28 at 5 31 21 PM](https://user-images.githubusercontent.com/109354592/192902041-a97b0e17-a23a-4baf-9ea8-c22bddb7e0ff.png)

<img width="663" alt="Movies_updated" src="https://user-images.githubusercontent.com/109354592/192901975-58747e5c-d6e3-49f2-a310-4fa010e1be32.png">

![Screen Shot 2022-09-28 at 5 40 18 PM](https://user-images.githubusercontent.com/109354592/192902015-797347c8-9ca8-4048-bf3b-c86d63a82f07.png)

<img width="667" alt="Ratings_updated" src="https://user-images.githubusercontent.com/109354592/192901986-120097c0-e76e-49f2-827e-5b5e0d58b18e.png">


## Summary
The ETL function collects & cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings csv files). The function transforms & merges  data, loads it into two updatable PostgreSQL dataset tables (provided) ready to be used by the hackathon participants for analysis.

