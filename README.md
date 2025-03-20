# Amazon Product Scraper

## Overview
This script scrapes product listings from Amazon using Selenium and BeautifulSoup. It collects information such as product name, price, rating, and number of reviews from multiple search result pages and saves the data in a CSV file.

## Features
- Scrapes multiple pages of Amazon search results
- Extracts product names, prices, ratings, and review counts
- Saves the data as a CSV file
- Uses Selenium with headless Chrome for automated browsing

## Requirements
Ensure you have the following installed before running the script:

- Python 3.x
- Google Chrome (latest version)
- ChromeDriver (managed via `webdriver-manager`)
- Required Python libraries:
  - `selenium`
  - `webdriver-manager`
  - `beautifulsoup4`
  - `pandas`

## Installation
1. Clone this repository or download the script.
2. Install dependencies by running:
   ```sh
   pip install selenium webdriver-manager beautifulsoup4 pandas
   ```
3. Ensure Chrome is installed on your system.

## Usage
Run the script using:
```sh
python amazon_scraper.py
```
By default, the script scrapes 3 pages of Amazon search results for "laptop" and saves the data in `amazon_products.csv`.

## Customization
- Modify the `scrape_amazon(pages=3)` function to change the number of pages scraped.
- Change the search keyword in the `url` inside the function.
- Modify the `extract_product_data()` function to extract additional product details.

## Legal Disclaimer
Scraping Amazon without permission may violate its [Terms of Service](https://www.amazon.com/gp/help/customer/display.html?nodeId=508088). Consider using the [Amazon Product Advertising API](https://affiliate-program.amazon.com/) for legal data access.

