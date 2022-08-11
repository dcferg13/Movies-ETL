# Movies-ETL
clean datasets of movie information
## Overview of Analysis
An updated analysis of the movie dataset, which has an automated pipeline of information that transforms raw data and loads into the existing tables. 
## Results
  - ETL Function
    - Wrote an ETL function that reads Wikipedia Data, Kaggle Data, and the MovieLens Data ratings and then put into three separate DataFrames. 
  - Extract and Transform Wikipedia Data
    - Took the raw Wikipedia data, extracted the information, and then transform it into a cleaner dataset. The first step was to clean up the alternate titles of the movies. Next, was to consolidate columns. Some of the columns had different names but had the same information. Example, being 'Edited By' and 'Editor(s)'. I also cleaned up rows, which had duplicates, removed columns that had null values, and lastly convert some of the datatypes (budget, box office, running time) into usable datatypes. 
  - Extract and Transform Kaggle Data
    - Take the raw Kaggle Data and cleaned it up to merge it with other datasets. First step was to remove bad data. Next step was to convert the data types. Lastly, was to check the ratings data and converting the timestamp into datatime data type. Also, in the ratings data we checked to see if there were any outliers in the actual ratings. 
  - Movie Database
    - The last step of this analysis was to take all the clean movie datasets and merge them into a singular dataframe and transfer it into a SQL database. 
## Summary	
  In summary, I took all the raw movie information from Wikipedia dataset, Kaggle Data and the MovieLens ratings data and cleaned it up into readable and functional datasets. Then merged all the datasets into one dataframe and made into a SQL database that will be easily accessible to those in the hackathon. The movies table has 6,052 rows and the ratings table has 26,024,289 rows. 
![ratings_query](https://user-images.githubusercontent.com/107289345/184228142-93f5499f-75e7-4086-8dc7-21296ed9f662.png)
![movies_query](https://user-images.githubusercontent.com/107289345/184228195-aff6d1ea-ddf1-4fa5-ae05-091f385e641c.png)
  

