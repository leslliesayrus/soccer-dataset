# data_of_soccer
I extracted 1800 maches of soccer from internet through the Selenium and I used the Pandas to processed them.

#  Data Ingestion

Using the Selenium and BeautifulSoup was made a Web Escraping to extract 1800 maches of soccer from site [1xbet](https://1xbet.whoscored.com/)
There's data of five different championships of 2021-2022 season:

Argentina 
Brazil
England
Italy
Spain

# Data Processing

Using Pandas DataFrame, its was joined the five files in only one table and making some settings, like create three new columns to 
indicate id a team win or not the specific match.

The file was saved in parquet (I saved in csv also for provide in Kaggle).


In the codes I used the service S3 from AWS to save the files and accesss them.
I used the Data Lake architecture to organize the data.
So the data are divided in ingestion layer (raw data from site) and curated layer (data processed in only one table).

