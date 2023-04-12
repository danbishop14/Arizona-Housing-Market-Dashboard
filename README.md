# Housing Market Dashboard

## Project Overview![Dashboard](https://user-images.githubusercontent.com/69700884/231599412-6123e305-0647-4427-912d-758e25f21253.JPG)


This project aims to analyze the housing market in Arizona's largest real estate markets. We extract data from Redfin's S3 bucket, clean and transform the data, and then load it into Power BI for visualization and analysis.


## Skills Used
- Data Extraction
- Data Cleaning
- Data Transformation
- Pandas (Python)
- Data Visualization (Power BI)


## How to use this project
- Extract Redfin Data: The script extracts Redfin data from the provided URL and stores it in a pandas DataFrame.
- Transform tables: The script cleans and transforms the data by slicing, mapping zip codes to cities, and merging the DataFrames.
- Load to Power BI: Save the transformed data as a CSV file to import it into Power BI for visualization and analysis.

## Setup and Installation
- Install Python 3.7 or higher.
- Install pandas library by running pip install pandas in your command prompt or terminal.
- Download the project files and extract them to a folder.
- Run the main.py script to extract, clean, and transform the data.
- Save the output CSV file and import it into Power BI for visualization.

Note: Power BI might not allow importing more than 2GB of data using a Python script. Ensure that the data being imported is within the allowed limit.

## Project Output
The project provides a cleaned and transformed CSV file containing Arizona housing market data, which can be used for analysis and visualization in Power BI.
