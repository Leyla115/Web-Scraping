web_sraping1.py query:

This script scrapes historical FIFA World Cup match results directly from Wikipedia for all tournaments between 1930–2022.

For each World Cup year, it:

Sends a request to the Wikipedia page for that tournament

Parses the HTML using BeautifulSoup

Extracts every match box (footballbox), including:

Home team

Score

Away team

Stores the results in a pandas DataFrame

Appends a year column for each match

Finally:

All tournaments are combined into a single DataFrame

Saved to fifa_worldcup_historical_data.csv

The 2022 tournament data is also saved separately as fifa_worldcup_fixture.csv

A custom User-Agent header is included to avoid Wikipedia’s bot restrictions.
