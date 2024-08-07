# FRED Economic Data Scraping Description

The script consists of a class `FREDAPIFetcher` to interact with the FRED API and fetch data for specified series. The main function, `fetch_gross_value_added_data`, retrieves GVA data for various sectors, processes the data, and saves it to a CSV file.

## FREDAPIFetcher Class

- **`__init__(self, api_key)`**: Initializes the class with the provided API key.
- **`fetch_series_data(self, series_id, start_date, end_date)`**: Fetches data for the specified series ID between the given start and end dates, processes the data into a pandas DataFrame, and returns it.

## fetch_gross_value_added_data Function

- **`fetch_gross_value_added_data(api_key)`**: Creates an instance of `FREDAPIFetcher`, defines the series IDs for various sectors, and fetches the data for each sector. The data is then combined into a single DataFrame and returned.

## Main Execution Block

- Replaces `'YOUR_API_KEY'` with your actual FRED API key.
- Calls `fetch_gross_value_added_data` and saves the resulting DataFrame to a CSV file.

## Instructions

### Set Up Your Environment

Ensure you have Python 3.x installed and the required libraries (`pandas` and `requests`) installed.

### Get Your FRED API Key

Sign up at [FRED](https://fred.stlouisfed.org/) to get an API key.

### Update the Script

Replace `'YOUR_API_KEY'` in the script with your actual FRED API key.
