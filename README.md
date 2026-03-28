## Overview

This tool automatically scrapes passenger reviews across all airlines listed on AirlineQuality.com. It extracts structured review data such as ratings, passenger types, travel routes, cabin class, and written feedback - making it useful for sentiment analysis, data science projects, or travel research.

---

## Features

- Scrapes reviews from all airlines listed A–Z on AirlineQuality.com
- Extracts structured data including ratings, routes, cabin class, and review text
- Handles pagination automatically
- Outputs clean, structured data ready for analysis

---

## Tech Stack

- **Python 3.x**
- **BeautifulSoup4** — HTML parsing
- **Requests** — HTTP requests
- **Pandas** — Data structuring and CSV export

---

## Usage
 
1. **Download** the `flightScraper.exe` file from the [Releases](../../releases) page
2. **Run** the executable and enter the name of the airline you want to scrape when prompted
 
Results are saved to a CSV file in the same directory as the executable.
 
---

## Output

The scraper saves data to `airline_reviews.csv` with columns such as:

| Column | Description |
|--------|-------------|
| `airline` | Name of the airline |
| `date` | Date of the review |
| `overall_rating` | Overall score out of 10 |
| `cabin_class` | Economy, Business, First, etc. |
| `route` | Origin and destination |
| `traveller_type` | Solo, Couple, Family, Business |
| `review_body` | Full text of the passenger review |
| `recommended` | Whether the reviewer recommends the airline |

> Column availability may vary depending on what individual reviewers filled in.

---

## Disclaimer

This project is intended for **educational and research purposes only**. Please review AirlineQuality.com's [Terms of Service](https://www.airlinequality.com) before use. Be respectful — avoid hammering the server with rapid requests. Consider adding delays between requests with `time.sleep()` if scraping at scale.

---

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to open a pull request or file an issue.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
