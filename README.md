# European Football League Data Analysis

## Introduction

This project aims to scrape and analyze data from the `understat.com` website for six European football leagues starting from the 2014/2015 season. The data includes metrics like expected goals (xG), expected goals against (xGA), and other statistical measures that help understand team performances over multiple seasons.

## Libraries Used

- `numpy`: Fundamental package for scientific computing with Python.
- `pandas`: Library providing high-performance, easy-to-use data structures and data analysis tools.
- `requests`: Non-GMO HTTP library for Python, safe for human consumption.
- `BeautifulSoup`: Library for pulling data out of HTML and XML files.

## Data Scraping

Data for the following leagues is scraped:

- La Liga
- EPL
- Bundesliga
- Serie A
- Ligue 1
- RFPL

For each league, data is collected by building a URL for each season and parsing the HTML content to extract JSON formatted data embedded within script tags.

## Data Structure and Processing

Data is stored in JSON format under the "script" tags as identified using Chrome Developer Tools. This data is then parsed into Python dictionaries and loaded into pandas DataFrames for further manipulation and analysis.

### Data Manipulation

- **Data Extraction**: Extract key performance metrics for each team for every match.
- **Aggregation**: Calculate total and average statistics across all matches for each team per season.
- **Comparison**: Generate additional metrics by comparing expected outcomes with actual outcomes, e.g., differences between expected goals and actual goals scored.

## Output

The analysis results in a detailed performance report for each team across each season, presented in pandas DataFrames and exported to CSV files for easy sharing and further analysis.

## Usage

To run this script, ensure you have Python installed along with the necessary libraries. Update the `base_url` if the structure of `understat.com` changes. You can execute the script from the command line or an IDE that supports Python scripts.

## Contributing

Contributions to this project are welcome. Please fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

