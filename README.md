Amazon Web Scraper
This project is a Python-based web scraper that extracts product information (such as title, author, rating, and price) from Amazon search results for books in Amharic. The data is scraped using BeautifulSoup and stored in a CSV file for further analysis.

Features
Extracts product links from the Amazon search results page.
Scrapes product details such as:
Title
Author
Rating
Price
Handles missing data gracefully and prints status messages for failed requests.
Saves the scraped data into a CSV file for further use.
Prerequisites
To run this project, you'll need the following installed:

Python 3.x
Required libraries:
BeautifulSoup4
requests
pandas
You can install the necessary libraries using pip:

bash
Copy code
pip install beautifulsoup4 requests pandas
How to Use
Clone this repository or download the source code.
Install the required Python libraries using the above command.
Open the Python script (amazon_scraper.py) and make sure the Amazon URL in the script matches your search query. Modify the URL variable as necessary.
Run the script:
bash
Copy code
python amazon_scraper.py
The script will scrape the product information and save it into a file called amazon_books.csv in the same directory.
Example Usage
By default, the script scrapes books in Amharic from the following search query:

arduino
Copy code
https://www.amazon.com/s?k=amharic+books&i=stripbooks-intl-ship
The extracted data includes:

Product Title
Author Name
Rating (if available)
Price (if available)
Project Structure
graphql
Copy code
├── final.py   # The main script for scraping Amazon
├── README.md           # This README file
├── test.py             # Test for single book
└── amazon_books.csv    # The output CSV file (generated after running the script)
Error Handling
If any product details (e.g., price or rating) are missing on a product page, the script will assign a default value such as N/A or No rating.
The script uses a 2-second delay between requests to avoid overwhelming Amazon's servers and to reduce the chances of being blocked.
Notes
Web scraping Amazon is subject to Amazon's Terms of Service. Please ensure you're scraping responsibly and within legal boundaries.
The class names in Amazon's HTML structure might change over time. You may need to adjust the class selectors in the script if scraping fails in the future.
License
This project is licensed under the MIT License. You are free to use, modify, and distribute it as you like.
