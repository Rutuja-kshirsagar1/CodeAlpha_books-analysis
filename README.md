# CodeAlpha_books-analysis

# 📘 Books-to-Insights — Web Scraping, EDA, and Visualization

## 🔍 Overview
Books-to-Insights is a beginner-friendly data analysis project that collects, cleans, and analyzes data from the website [Books to Scrape](http://books.toscrape.com/).  
It walks through every step of a real-world data science workflow — from data collection to storytelling.

The project focuses on exploring questions like:
- Do higher-rated books cost more?
- What’s the overall price distribution?
- Are there any pricing or rating anomalies?

---

## 🚀 Project Workflow

### 1. Web Scraping
- **Tools used:** `requests`, `BeautifulSoup`
- Scraped book details from all pages, including:
  - Title  
  - Price (£)  
  - Rating (1–5 stars)  
  - Availability status  
- Exported raw data to `books_raw.csv`.

### 2. Data Cleaning
- Removed unwanted symbols (e.g., `Â`, `£`)
- Cleaned availability text
- Handled missing ratings
- Created new feature: `price_bin`
- Saved cleaned dataset as `books_clean.csv`

### 3. Exploratory Data Analysis (EDA)
- Summary statistics of prices and ratings  
- Distribution plots and outlier detection  
- Average price per rating  
- Visual patterns between price and rating  

### 4. Hypothesis Testing
- **Hypothesis:** Higher-rated books have higher prices.  
- **Tests performed:**
  - Spearman correlation → measures monotonic relation between rating & price.  
  - Independent t-test → compares average prices of high-rated vs low-rated books.  

### 5. Visualization
- Histograms, boxplots, and heatmaps created using **Matplotlib** and **Seaborn**.  
- Example visuals:
  - Price Distribution
  - Boxplot of Price vs Rating
  - Correlation Heatmap  

---

## 🧰 Tools & Libraries
| Purpose | Libraries / Tools |
|----------|-------------------|
| Web Scraping | `requests`, `BeautifulSoup` |
| Data Handling | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn` |
| Statistics | `scipy.stats` |

# 📊 Results & Insights
- Most books are priced between **£20–£50**.  
- Weak but positive correlation between **rating and price** (higher-rated books tend to cost slightly more).  
- A few high-priced outliers were found but not directly tied to rating.  
- Data cleaning significantly improved the quality of insights.

- # 🧠 Key Learning Outcomes
- Understand HTML structure and extract data programmatically.
- Clean and preprocess real-world messy data.
- Ask analytical questions and test hypotheses statistically.
- Create visuals that reveal insights effectively.
- Document and present a full data project professionally.

