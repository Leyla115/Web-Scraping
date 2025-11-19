	web_scraping1.py

This script scrapes historical FIFA World Cup match results from Wikipedia for all tournaments between 1930–2022.

How it works

For each World Cup year, it:

Sends an HTTP request to that year’s Wikipedia page

Parses the HTML content with BeautifulSoup

Extracts every match container (footballbox), including:

	Home team
	
	Score
	
	Away team

Stores the extracted data in a pandas DataFrame

Adds a year column to each record

	Output

All tournaments are combined into a single dataset and saved as:
fifa_worldcup_historical_data.csv

The 2022 tournament is scraped separately and saved as:
fifa_worldcup_fixture.csv

	A custom User-Agent header is included to avoid Wikipedia bot-blocking.
