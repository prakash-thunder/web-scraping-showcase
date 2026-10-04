# 🌍 Population Table Web Scraping

A Python project demonstrating how to extract a complete **HTML table** from a webpage using BeautifulSoup and convert it into a Pandas DataFrame.

## 🔎 Source

The notebook extracts the population-by-country table from the Worldometer webpage used in the project.

## 📊 Data extracted

The final CSV contains **234 rows** and includes fields such as:

- Country / dependency
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

## 🛠️ Libraries

```python
import requests
from bs4 import BeautifulSoup
import pandas as pd
import numpy as np
```

## 🔄 Process

```text
Webpage
   ↓
HTTP request
   ↓
BeautifulSoup
   ↓
Locate <table>
   ↓
Extract <th> headers
   ↓
Extract <tr> / <td> rows
   ↓
NumPy array
   ↓
Pandas DataFrame
   ↓
CSV
```

## ▶️ Run

Open:

`population_table_scraping.ipynb`

and execute the notebook from top to bottom.

## 📂 Files

| File | Description |
|---|---|
| `population_table_scraping.ipynb` | Complete table scraping notebook |
| `Countries_in_the_world_by_population.csv` | Scraped population dataset |
