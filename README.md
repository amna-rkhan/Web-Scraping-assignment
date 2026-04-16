# Project Name: Books to Scrape Data Collector

### 1. Project Overview
* **Target Website:** http://books.toscrape.com/
* **Data Fields Extracted:** Title, Price, Availability
* **Tools Used:** Python, BeautifulSoup, Pandas, Requests

### 2. Setup Instructions
1. Clone this repo: `git clone https://github.com/amna-rkhan/Web-Scraping-assignment.git`
2. Install dependencies: `pip install -r required.txt`
3. Run script: `python web.py`

### 3. Challenges & Solutions
* **Challenge:** The availability field contained a lot of unnecessary whitespace and hidden newlines.
* **Solution:** I used the `.strip()` method in Python to clean the strings before appending them to the list, ensuring the final CSV was professional and "clean."
