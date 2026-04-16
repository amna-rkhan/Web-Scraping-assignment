Data Acquisition Project
Overview
This project automates the collection of e-commerce data using BeautifulSoup. The goal was to build a reliable data pipeline to extract product information for future analysis.

Target: Books to Scrape

Output: data2.csv

Technical Stack
BeautifulSoup4: For HTML parsing and tag extraction.

Requests: For handling HTTP connections.

Pandas: For structuring data into a CSV format.

Execution Logic
Request: Fetch the HTML source of the target webpage.

Parse: Locate product containers using the <article> tag and product_pod class.

Extract: Capture the Title and Price for each item.

Save: Export the gathered list into a structured DataFrame and save as data2.csv.

Challenges Faced
Initial attempts to scrape JavaScript-heavy sites (like Daraz) resulted in empty datasets. I successfully pivoted to a server-side rendered site to ensure 100% data integrity and a stable pipeline for this assignment.
