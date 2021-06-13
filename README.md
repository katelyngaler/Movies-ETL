# Movies-ETL

The purpose of this analysis was to work with cleaning data in the process known as ETL (Extract, Transform, and Load). We looked at movie data from multiple sources, cleaned the data, merged the tables, and loade it into PostGreSQL.

The 4 deliverables include:
1. Reading the data  (ETL_function_test.ipynb)
2. Extract and transform the wikipedia data (ETL_clean_wiki_movies.ipynb)
    * TV shows are filtered out
    * Try/Except is used to catch errors while parsing imdb IDs
    * BOx office data is converted to strings, scubbed to be standard format, then changed to float
    * Box office, budget, release data, and running time all transformed
    * Create dataframe
3. Extract and transform the kaggle data (ETL_clean_kaggle_data.ipynb)
    * Kaggle data is cleaned, filtered, strings converted to numbers/dates where applicable
    * Kaggle and wiki dataframes are merged, combine data, remove extra columns
    * Rating data is transformed with pivot
    * Rating data is merged with kaggle/wiki df
4. Load the transformed data into the movie database (ETL_create_database.ipynb, and 2 images in resources folder)
    * movies_df and ratings csv are imported into SQL