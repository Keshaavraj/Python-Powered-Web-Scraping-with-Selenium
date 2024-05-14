# Web Scraping using Selenium

## Introduction
🔍 This project demonstrates web scraping using Selenium, a Python library commonly used for automating web browsers. The code scrapes job listings from a popular job portal, Naukri.com, specifically targeting data scientist roles. The extracted data is then processed and saved into a CSV file for further analysis.

## Table of Contents
- [Setup](#setup)
- [Scraping](#scraping)
- [Pre-Processing](#pre-processing)
- [Saving](#saving)

## Setup
Ensure you have the necessary libraries installed before running the script. You can install them via pip:

```bash
pip install selenium pandas beautifulsoup4
```

Additionally, download the appropriate WebDriver for your browser. In this script, Chrome WebDriver is used. Ensure the WebDriver executable is in the system path or provide the path in the code.

## Scraping
The scraping process involves automating the browser to navigate to Naukri.com and fetching job listings for data scientist roles. Here's a breakdown of the scraping process:
- Load necessary libraries
- Initialize the Selenium WebDriver
- Define a dictionary to store job details
- Iterate through multiple pages of job listings
- Extract job details such as title, company, location, experience, skills, salary, etc., using CSS selectors
- Handle exceptions for missing data
- Append job details to the dictionary
- Transform the dictionary into a Pandas DataFrame

## Pre-Processing
Pre-processing steps are applied to clean and format the extracted data:
- Convert all strings to lowercase to avoid redundancy
- Split multiple locations and skills associated with each job listing
- Check for and drop any missing values in the DataFrame

## Saving
The processed data is saved into a CSV file named `Page251-252.csv` for further analysis.

## Usage
To run the script:
1. Ensure the WebDriver executable is available in the system path or provide the path in the code.
2. Execute the Python script `web_scraping.py`.

## Dependencies
- Selenium
- Pandas
- BeautifulSoup

## Contributing
Pull requests and contributions are welcome. For major changes, please open an issue first to discuss what you would like to change.

