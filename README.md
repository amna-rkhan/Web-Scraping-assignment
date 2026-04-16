# Project Name: Shopify eCommerce Data Extractor

### 1. Project Overview
* **Target Website:** [(https://www.allbirds.com/products.json)]
* **Data Fields Extracted:** Product Title, Price, Product Type
* **Tools Used:** Python, Requests, JSON, Pandas

### 2. Project Structure
* `web.py`: The main Python script utilizing the Shopify JSON API for extraction.
* `data3.csv`: The final dataset containing the exported product information.
* `requirements.txt`: List of necessary Python libraries.
* `README.md`: Project documentation.

### 3. Setup Instructions
1. Clone this repo: `git clone https://github.com/amna-rkhan/Web-Scraping-assignment.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run script: `python web.py`

### 4. Challenges & Solutions
* **Technical Hurdle:** Traditional HTML scraping using BeautifulSoup can be fragile if the website theme changes or uses heavy JavaScript (like Wix or Shopify).
* **The Solution:** I pivoted to using Shopify's native JSON endpoint (`/products.json`). This allowed for more reliable data extraction, bypassed the need for complex CSS selectors, and ensured 100% data accuracy in the final CSV.
* **Ethical Scraping:** I implemented a `time.sleep(1)` delay in the extraction loop to ensure the script respects the server's rate limits.
