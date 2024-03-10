# YouTube Data Harvesting and Warehousing.

## Introduction 

* YouTube, the online video-sharing platform, has revolutionized the way we consume and interact with media. Launched in 2005, it has grown into a global phenomenon, serving as a hub for entertainment, education, and community engagement. With its vast user base and diverse content library, YouTube has become a powerful tool for individuals, creators, and businesses to share their stories, express themselves, and connect with audiences worldwide.

* This project extracts the particular youtube channel data by using the youtube channel id, processes the data, and stores it in the MongoDB database. It has the option to migrate the data to PostgreSQL from MongoDB then analyse the data and give the results depending on the customer questions.


## Developer Guide 

### 1. Tools Install

* Jupyter notebook.
* Python 3.11.0 or higher.
* PostgreSQL.
* MongoDB.
* Youtube API key.

### 2. Requirement Libraries to Install

* pip install google-api-python-client.
  
* pip install pymongo.
    
* pip install psycopg2. 
    
* pip install pandas.

* pip install streamlit.

  
### 3. Import Libraries

**Youtube API libraries**
* import googleapiclient.discovery
* from googleapiclient.discovery import build

**MongoDB**
* import pymongo

**SQL libraries**
* import psycopg2

**pandas**
* import pandas as pd


**Dashboard libraries**
* import streamlit as st

### 4. E T L Process

#### a) Extract data

* Extract the particular youtube channel data by using the youtube channel id, with the help of the youtube API developer console.

#### b) Process and Transform the data

* After the extraction process, takes the required details from the extraction data and transform it into JSON format.

#### c) Load  data 

* After the transformation process, the JSON format data is stored in the MongoDB database, also It has the option to migrate the data to MySQL database from the MongoDB database.

### 5. E D A Process and Framework

#### a) Access PostgreSQL DB 

* Create a connection to the PostgreSQL server and access the specified PostgreSQL DataBase by using psycopg2 library and access tables.

#### b) Filter the data

* Filter and process the collected data from the tables depending on the given requirements by using SQL queries and transform the processed data into a DataFrame format.

###  6. Data Visualization

* Visualize the collected data from the tables by using the plotly.express and transform the processed data into a chart format to understand easily.

