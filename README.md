# Scrape Sustainalytics ratings from Yahoo! Finance
Python3 script to scrape all available Sustainalytics ratings from Yahoo! Finance for stocks and ETFs. As the Yahoo! Finance website uses mostly javascript, scraping is done using Selenium. 

## Dependencies
1. bs4 / BeautifulSoup 4 (`!pip install beautifulsoup4`)
2. selenium (`!pip install selenium`)
2. pandas (comes pre-installed with Anaconda, otherwise `!pip install pandas`)
3. numpy (comes pre-installed with Anaconda, otherwise `!pip install numpy`)
4. re (comes pre-installed)
5. time (comes pre-installed)

## Outputs
The script outputs 2 .csv files:	

* `yahoo_finance_sustainalytics_tickers.csv`: contains all tickers and company names for which ESG data is available (the universe)		
* `yahoo_finance_sustainalytics.csv`: the ESG risk ratings, controversy levels, and product involvement flags for the ESG stock universe	
