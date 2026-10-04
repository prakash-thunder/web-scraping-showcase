# 🕷️ Web Scraping with Python

A collection of Python web scraping projects using **Requests, BeautifulSoup, Pandas, and NumPy**.

> **Web → HTML → BeautifulSoup → Data Extraction → Pandas → CSV**

## 📌 Projects

| Project | Description | Tools |
|---|---|---|
| 📚 [Books Web Scraping](./01_books_web_scraping/) | Scrapes book details from 50 catalogue pages | Requests, BeautifulSoup, Pandas |
| 🌍 [Population Table Scraping](./02_population_table_scraping/) | Extracts population data from an HTML table | Requests, BeautifulSoup, Pandas, NumPy |

## 📚 Books Web Scraping

Scrapes **1,000 books** across 50 catalogue pages.

**Extracted:** Book name, price, rating, stock, and URL.

**Output:** `Book_info_all.csv`

[View Project →](./01_books_web_scraping/)

## 🌍 Population Table Scraping

Extracts a structured population table from a webpage and converts it into a Pandas DataFrame.

**Extracted:** Population, yearly change, density, land area, migrants, fertility rate, median age, and more.

**Output:** `Countries_in_the_world_by_population.csv`

[View Project →](./02_population_table_scraping/)

## 🛠️ Tech Stack

```text
Python
├── Requests
├── BeautifulSoup4
├── Pandas
└── NumPy
