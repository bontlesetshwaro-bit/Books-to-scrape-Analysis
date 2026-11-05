# Books to Scrape - Price Analysis

## Overview
This project scrapes book data from **books.toscrape.com**, cleans the dataset,
and analyses how book prices relate to ratings, availability, and category.

A total of **1000 books** were scraped across all 50 pages of the site.

**GitHub Repository:** https://github.com/bontlesetshwaro-bit/Books-to-scrape-Analysis

## Objectives
1. Scrape 1000 books including title, price, rating, availability, and category.
2. Clean and prepare the data for analysis.
3. Visualise price patterns and trends.
4. Test the relationship between price, rating, and availability using correlation and regression.

## Tools Used
- **Python** - programming language
- **BeautifulSoup & Requests** - web scraping
- **Pandas & NumPy** - data cleaning and analysis
- **Matplotlib & Seaborn** - data visualisation
- **Scikit-learn** - correlation and linear regression
- **Jupyter Notebook / PyCharm** - development environment

## Files in this Repository
| File | Description |
| --- | --- |
| `Books to scrape Analysis.ipynb` | Main notebook: cleaning, 7 visuals, correlation, regression |
| `books_scraped_dataset.csv` | Cleaned dataset with 1000 books |
| `script.py` | Python script used to scrape the data |

## Methodology

### 1. Data Collection (Scraping)
- Scraped all 50 pages from books.toscrape.com
- For each book collected: Title, Price (£), Rating (1-5 stars), Availability, Category, and URL
- Saved raw data to CSV

### 2. Data Cleaning
- Removed duplicate books
- Converted Price from text (e.g. "£51.77") to numeric
- Converted Rating from words (e.g. "Three") to numbers (1-5)
- Converted Availability to In Stock / Out of Stock
- Checked for missing values - no missing values found
- Final dataset: 1000 rows

### 3. Exploratory Data Analysis (7 Visuals)
1. Distribution of Book Prices (Histogram)
2. Average Price by Rating (Bar Chart)
3. Average Price by Category - Top 10 (Bar Chart)
4. Price vs Rating (Box Plot)
5. Availability of Books (Pie Chart)
6. Price vs Rating (Scatter Plot)
7. Correlation Heatmap

### 4. Correlation and Regression
- **Correlation:** Pearson correlation between Price and Rating
- **Regression:** Simple Linear Regression to predict Price from Rating
- Evaluated using R-squared and p-value

## Key Findings
- Most books are priced between £10 and £40, with a few expensive outliers above £50.
- Higher-rated books do NOT always cost more - price is influenced more by category than by rating.
- [Add your exact correlation value here, e.g. Correlation between Price and Rating = 0.12]
- [Add your exact regression result here, e.g. R-squared = 0.01, meaning rating explains very little of price variation]
- Travel and Mystery categories had some of the highest average prices, while [add lowest category] had the lowest.

> Tip: Open the notebook to see the exact numbers in the output cells.

## How to Run This Project
1. Clone the repository: