# 📚 Books Web Scraping

A Python web scraping project using **Requests + BeautifulSoup + Pandas** to collect book information from Books to Scrape.

## 🔎 What is scraped?

For each book:

- Book name
- Book link
- Price
- Stock availability
- Rating

## 📊 Two scraping versions

### Single page

The notebook first scrapes the first catalogue page and stores the result in:

`Book_info.csv`

### All pages

The scraper then loops through pages **1–50** and collects the complete catalogue:

`Book_info_all.csv`

The final dataset contains **1,000 books**.

## 🛠️ Libraries

```python
import requests
from bs4 import BeautifulSoup
import pandas as pd
```

## 🔄 Process

```text
Request webpage
      ↓
Parse HTML with BeautifulSoup
      ↓
Find book elements
      ↓
Extract name / price / stock / rating / link
      ↓
Create DataFrame
      ↓
Save CSV
```

## ▶️ Run

Open:

`books_web_scraping.ipynb`

and run the cells from top to bottom.

## 📂 Files

| File | Description |
|---|---|
| `books_web_scraping.ipynb` | Complete scraping notebook |
| `Book_info.csv` | First-page scraped data |
| `Book_info_all.csv` | All 1,000 scraped books |
