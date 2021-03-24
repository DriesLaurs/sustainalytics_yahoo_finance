# Scrape Sustainalytics ratings from Yahoo! Finance
Python3 script to scrape all available Sustainalytics ESG ratings from Yahoo! Finance for stocks and ETFs. As the Yahoo! Finance website loads JavaScript, scraping is done using Selenium. Note that for getting Selenium to work, you need to install a webdriver. I used [ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/downloads). 

### IMPORTANT: USE AT YOUR OWN RISK. SCRAPING MAY BE AGAINST YAHOO!'s TERMS OF SERVICE.

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
* `yahoo_finance_sustainalytics.csv`: the ESG risk ratings, controversy levels, and product involvement flags for stocks and ETFs in the universe
