# Medibaze

This project aims to download drug availability data from the www.sukl.cz website's API, which provides information about the availability of drugs in the Czech Republic. The downloaded data includes unique SUKL codes that represent specific drugs but there are not drug names. The project utilizes web scraping techniques to extract the necessary data and create a custom JSON file that maps SUKL codes to their corresponding drug names.

**Note: This project is currently under development.**

## Important files:

1. ```get_api_data.py
- Downloads new API data to datayyyy-mm-dd.json file
- Compares old data and new data to get unknown SUKL codes

2. ```pairing_sukl_names/scraper.py
- Opens list of unknown SUKL codes to be scraped
- Scrapes names
- Matches scraped names to unknown SUKL codes
- Makes update to vsechny_nazvy.json file
