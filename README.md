# Web-Scraper

# 🖥️ Newegg Product Price Scraper

A Python script to scrape product listings, prices, and links from [Newegg Canada](https://www.newegg.ca) based on your search term. This script retrieves all results across multiple pages and prints product details in your terminal.

## Requirements

Make sure you have Python installed, and then install the required libraries:

```bash
pip install beautifulsoup4 requests
```

## Usage

1. **Run the Script**
    ```bash
    python script_name.py
    ```
2. **Enter a Product**
    - When prompted, type your desired product (e.g., `RTX 3080`, `laptop`, etc.).

3. **View the Results**
    - The script prints product name, price, and Newegg link for each listing.

**Example Output:**
```
ASUS ROG Strix RTX 3060 Gaming GPU
$549
https://www.newegg.ca/...
-------------------------------
```
---

## Customization: Using Other Websites

To adapt this script for other e-commerce websites:

1. **Change the Search URL**  
   Replace the Newegg URL patterns with the search URL of the target website.

2. **Update HTML Selectors**  
   Use your browser’s developer tools to inspect the site’s structure and adjust class names and tags accordingly. Look for product title, price, and link containers.

3. **Adjust Extraction Logic**  
   If prices or product names are split across different tags or formatted differently, modify the data parsing code to extract them robustly.

**Tip:** Many sites require you to set a `User-Agent` in headers:
```python
headers = {"User-Agent": "Mozilla/5.0 ..."}
requests.get(url, headers=headers)
```

> **Note:**  
> This script is designed around Newegg’s website structure as of now. Websites change - if extraction breaks, double-check HTML classes/tags.

## Suggestions & Improvements

- Save results to CSV or JSON.
- Add delays to avoid rate-limiting.
- Handle errors more gracefully.
- Build a simple GUI using Tkinter or web app with Flask.
- For JavaScript-heavy sites, try Selenium.

## Disclaimer

This script is for learning and personal use only. Always respect websites’ terms of service and robots.txt rules when scraping.

You’re all set! Paste this as your repository’s `README.md` and modify as needed.
