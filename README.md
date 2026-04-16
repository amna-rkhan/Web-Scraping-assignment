Data Acquisition & Web Scraping Project

Project Overview
Target Website: Books to Scrape

Dataset: 20+ records of product metadata (Titles, Prices, Availability).

Output: data2.csv (Ready for exploratory data analysis).

Data Engineering Pipeline
To ensure a high-quality dataset, the following scraping pipeline was implemented:

Library Stack: BeautifulSoup4 for HTML parsing and Requests for HTTP communication.

Extraction Logic: Utilized BeautifulSoup’s CSS selectors to navigate the DOM tree and extract nested attributes within article tags.

Data Transformation: Leveraged Pandas to clean raw strings (removing whitespace and non-numeric characters) and structure them into a tabular format.

Technical Challenges & Robustness
In Data Science, data reliability is paramount. This project involved significant troubleshooting:

Handling Dynamic Content: I initially tested high-volume platforms like Daraz and Dribbble. However, I identified that these sites use Client-Side Rendering (JavaScript), which led to incomplete datasets when using static scrapers.

The Solution: I pivoted to Books to Scrape, a server-side rendered site. This decision was made to ensure 100% data extraction success and to demonstrate a stable, reproducible data pipeline.

Ethical Data Collection: To prevent server-side rate-limiting and practice ethical data acquisition, a 1-second latency (time.sleep) was added between requests.

