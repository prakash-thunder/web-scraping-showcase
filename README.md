# 🕷️ Web Scraping with Python & BeautifulSoup

A practical collection of **Python web scraping projects** built with **Requests, BeautifulSoup, Pandas, and NumPy**.

This repository demonstrates two common real-world scraping tasks:

- 📚 **Scraping product-style website data** from multiple pages
- 🌍 **Extracting structured data from an HTML table** and exporting it to CSV

The focus is on understanding the complete workflow:

**Website → HTTP Request → HTML → BeautifulSoup → Data Extraction → Pandas → CSV**

---

## ✨ Projects

| Project | What it does | Main tools |
|---|---|---|
| 📚 [Books Web Scraping](./01_books_web_scraping/) | Scrapes book name, price, stock, rating and links from Books to Scrape | Requests, BeautifulSoup, Pandas |
| 🌍 [Population Table Scraping](./02_population_table_scraping/) | Extracts a country population table from a webpage and saves it as CSV | Requests, BeautifulSoup, Pandas, NumPy |

---

## 📚 01 — Books Web Scraping

**Source:** Books to Scrape

The project starts by scraping one page and then scales the same approach to all **50 catalogue pages**.

### Data collected

- Book name
- Book link
- Price
- Stock availability
- Rating

### Output

- `Book_info.csv` — first-page sample
- `Book_info_all.csv` — complete scraped catalogue

**Dataset size:** 1,000 books.

### Workflow

```text
Books to Scrape
      ↓
requests.get()
      ↓
BeautifulSoup
      ↓
Find book cards
      ↓
Extract fields
      ↓
Pandas DataFrame
      ↓
CSV
```

👉 [Open the Books scraping project](./01_books_web_scraping/)

---

## 🌍 02 — Population Table Scraping

**Source:** Worldometer population-by-country page

This project demonstrates how to scrape an existing HTML `<table>` rather than individual cards.

### Data collected

The resulting dataset contains country/dependency information including:

- Population
- Yearly Change
- Net Change
- Density
- Land Area
- Migrants
- Fertility Rate
- Median Age
- Urban Population
- World Share

**Rows extracted:** 234 countries/dependencies.

### Workflow

```text
Population webpage
      ↓
requests.get()
      ↓
BeautifulSoup
      ↓
Locate HTML table
      ↓
Extract headers + rows
      ↓
NumPy / Pandas
      ↓
CSV
```

👉 [Open the population table project](./02_population_table_scraping/)

---

## 🧰 Tech Stack

```text
Python
├── Requests
├── BeautifulSoup4
├── Pandas
└── NumPy
```

---

## 🧠 What I Practiced

Through these projects, I worked with:

- HTTP requests
- HTML parsing
- CSS/HTML element selection
- BeautifulSoup
- Multi-page scraping
- HTML table extraction
- DataFrame creation
- Basic data transformation
- Converting scraped data into CSV
- Structuring scraped data for further analysis

---

## 🚀 Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/web-scraping-showcase.git
cd web-scraping-showcase
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Start Jupyter Notebook

```bash
jupyter notebook
```

Then open either:

```text
01_books_web_scraping/books_web_scraping.ipynb
```

or

```text
02_population_table_scraping/population_table_scraping.ipynb
```

---

## 📁 Repository Structure

```text
web-scraping-showcase/
│
├── 📚 01_books_web_scraping/
│   ├── books_web_scraping.ipynb
│   ├── Book_info.csv
│   ├── Book_info_all.csv
│   └── README.md
│
├── 🌍 02_population_table_scraping/
│   ├── population_table_scraping.ipynb
│   ├── Countries_in_the_world_by_population.csv
│   └── README.md
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## ⚠️ Note

These projects are created for **learning and practicing web scraping and data collection with Python**.

Always check a website's terms of use and `robots.txt`, and scrape responsibly.

---

## 👤 Author

**Prakash Kumar**

Interested in **Data Science, Python, Machine Learning, and Data Engineering**.

⭐ If you find this repository useful, consider giving it a star.
