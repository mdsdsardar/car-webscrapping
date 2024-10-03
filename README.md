Project Overview
This project scrapes car listings from a website and extracts important information such as:
Year of manufacturing
Car maker (brand)
Car model
Distance driven (km driven)
Fuel type (petrol, diesel, etc.)
Transmission type (manual/automatic)
Price of the car
Location of the listing
The fetched data is organized into a pandas DataFrame for easy analysis and can be exported to CSV, Excel, or any other format.

Required Libraries:
pandas: For creating and manipulating DataFrames.
BeautifulSoup: For parsing and extracting HTML content.
requests: For sending HTTP requests and fetching web pages.

Code Overview
The main components of the script are:

HTTP Request: The requests library is used to fetch HTML content from the target website.

HTML Parsing: The BeautifulSoup library parses the HTML and identifies elements (e.g., car models, prices, locations) based on their HTML tags and classes.

Data Extraction: The relevant data points (year, car model, etc.) are extracted from the HTML and stored in the pandas DataFrame.

DataFrame Structure: The DataFrame has the following columns: 'year', 'car_makers', 'car_model', 'km_driven', 'fuel_type', 'transmission', 'price', 'location'.

Data Columns
The DataFrame consists of the following columns:
year: Year the car was manufactured.
car_makers: The manufacturer of the car (e.g., Toyota, Honda).
car_model: The specific model of the car.
km_driven: The total kilometers the car has been driven.
fuel_type: The type of fuel the car uses (e.g., Petrol, Diesel).
transmission: The type of transmission (Manual or Automatic).
price: The price of the car.
location: The location where the car is being sold (e.g., Gurugram).
