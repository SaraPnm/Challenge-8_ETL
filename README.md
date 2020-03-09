# Challenge 8, ETL

## Project Overview
We will write a Python script that performs all three ETL steps on the Wikipedia and Kaggle data.

The goals of this challenge are to:

1. Create an automated ETL pipeline.
2. Extract data from multiple sources.
3. Clean and transform the data automatically using Pandas and regular expressions.
4. Load new data into PostgreSQL.

## Resources
- Data Source: ratings.csv & movies_metadata.csv
- Software: Python 3.6.1, Jupyter Notebook

# Summary
A function is created that takes in three arguments and performs all of the transformation steps:
- Wikipedia data
- Kaggle metadata
- MovieLens rating data (from Kaggle)

Here are a few assumptions made in this challenge:
1. a movie without imdb_link and director name gets removed from the list.
2. Selected data formats are accepted for different columns. Any additional regular expressions not in this code may need to be added in the future.
3. All the columns with more than 90% of null values get removed from the data analysis.
4. Input data are in the origin master with specific formats defined in the csv files.
5. Any additional movie languages not defined in the code should be added if necessary.
