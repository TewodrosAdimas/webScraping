### Enhancements:

1. Add a **Dependencies** section under _Prerequisites_ for clarity.
2. Ensure consistency by specifying the filename in the _Modify the Amazon URL_ step.
3. Mention a troubleshooting tip in case the script doesn't work.

---

### Updated README:

````markdown
# Amazon Web Scraper

This Python-based project scrapes product information (title, author, rating, and price) from Amazon search results for books in Amharic. Using BeautifulSoup, it extracts data and stores it in a CSV file for further analysis.

---

## Features

- Extracts product links from Amazon search results pages.
- Scrapes product details such as:
  - **Title**
  - **Author**
  - **Rating**
  - **Price**
- Handles missing data gracefully and logs the status of failed requests.
- Saves scraped data into a CSV file for further use.

---

## Prerequisites

Ensure you have the following installed before running the project:

- **Python** (version 3.5 or above)
- Required libraries:
  - `beautifulsoup4`
  - `requests`
  - `pandas`

### Dependencies

Install the required libraries by running:

```bash
pip install -r requirements.txt
```
````

---

## Installation and Usage

1. **Clone or download the repository**:

   ```bash
   git clone https://github.com/TewodrosAdimas/webScraping.git
   cd webScraping
   ```

2. **Install the required Python libraries**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Modify the Amazon URL in the script**:  
   Open `final.py` in a text editor and update the `URL` variable to match your search query.

4. **Run the script**:

   ```bash
   python final.py
   ```

5. **Output**:  
   The scraped product information will be saved to a file named `amazon_books.csv` in the project directory.

---

## Project Structure

```plaintext
├── final.py          # Main script for scraping Amazon
├── README.md         # Documentation (this file)
├── requirements.txt  # Python dependencies
```

---

## Error Handling

- If product details (e.g., price or rating) are missing, the script assigns default values such as `N/A` or `No rating`.
- Implements a **2-second delay** between requests to avoid overwhelming Amazon's servers and reduce the likelihood of being blocked.

---

## Notes

- **Respect Amazon's Terms of Service**:  
  Scraping Amazon is subject to their Terms of Service. Ensure you scrape responsibly and within legal boundaries.

- **HTML structure changes**:  
  Amazon's class names and structure might change over time. If the scraper stops working, update the class selectors in the script.

- **Troubleshooting**:  
  If you encounter errors while running the script:
  - Ensure your Python version and dependencies are correctly installed.
  - Verify the Amazon URL in `final.py`.

---

## License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute it as you like.

---

```

```
