# Real Estate Data Analysis
This Python script is used to download real estate data from Redfin and perform data transformation to prepare the data for analysis. The data is then used to create a PowerBI dashboard for further analysis.

## Data Source
The data is obtained from Redfin, which is a real estate company that provides a variety of real estate data through its Data Center. The specific URL for the data used in this script is:

## Copy code
https://redfin-public-data.s3.us-west-2.amazonaws.com/redfin_market_tracker/zip_code_market_tracker.tsv000.gz
## Data Transformation Steps
1. Retrieve the entire Redfin data set from the specified URL.
2. Create a new table to map zip codes to county/city using data from the following URL: https://raw.githubusercontent.com/scpike/us-state-county-zip/master/geo-data.csv
3. Select only the data for the state of Arizona.
4. Clean and transform the data by:
- Extracting the zip code from the region column and converting it to an integer.
- Calculating the month-over-month change in median days on market (median_dom_mom) by sorting the data by period_begin and applying the pct_change function.
- Merging the two tables on the zipcode column.
- Dropping unnecessary columns and renaming others for clarity.
## Output
The resulting data frame, az_redfin_df, is then used as input for a PowerBI dashboard for further analysis.
