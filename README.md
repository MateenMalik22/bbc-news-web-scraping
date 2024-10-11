# **BBC News Web Scraping Project**

## **Project Overview**
This project involves web scraping news articles from the BBC News website to gather **headlines**, **categories**, **timestamps**, and **author information**. The objective is to collect, organize, and analyze this data for insights, and store it in a structured **CSV** format for further use.

---

## **Objective**
- **Scrape** news data from BBC News, including **headlines**, **categories**, **authors**, and **timestamps**.
- **Organize** the data in a well-structured **CSV** file for ease of analysis and visualization.
- **Analyze** trends, such as the most frequent categories, to understand BBC's focus areas.

---

## **Usage**
The project can be used to:
- **Analyze the distribution** of news categories and understand publication patterns.
- Provide **organized data** in a CSV format for further analysis or sharing.

---

## **Challenges & Solutions**
- **Handling HTML Variability**: The HTML structure of news pages often changes, making scraping challenging. This was managed by **thorough inspection** and adding **error handling** to deal with unpredictable formats.
- **Data Accuracy**: Missing or inconsistent data was managed by **cleaning the dataset**, including removing rows with missing values in critical columns and converting timestamps.

---

## **Future Scope**
- **Extend the Project**: Scrape news from other websites to gain broader insights.
- **Automate Scraping**: Automate the process for real-time scraping and analysis to track news trends over time.

---

## **Technologies and Tools Used**
- **Programming Language**: Python
- **Libraries**:
  - `requests`: To send HTTP requests and retrieve HTML content.
  - `BeautifulSoup`: For parsing HTML and extracting data like headlines and categories.
  - `pandas`: To organize extracted data into a DataFrame and export it to CSV.
  - `lxml`: Used as an HTML parser.
  - `matplotlib`: For visualizing data (e.g., top categories).
- **IDE**: Google Colab for executing and developing the code.

---

## **Web Scraping Process**
1. **Sending HTTP Requests**: Used `requests` to fetch HTML content from BBC News.
2. **Parsing HTML**: Extracted relevant elements (e.g., headlines, categories) using `BeautifulSoup`.
3. **Data Cleaning**:
   - **Dropped Author Column**: Due to insufficient data.
   - **Converted Timestamp**: Into a date-time format for easy analysis.
   - **Removed Rows with Missing Values**: Cleaned data by dropping rows with missing values in critical columns like `Category` and `Timestamp`.
4. **Data Storage**: Organized the cleaned data into a **CSV file** for easy sharing and analysis.

---

## **Data Analysis and Visualization**
- Generated **visuals** (e.g., bar chart) to highlight the **Top 5 News Categories** from the scraped data.
- **Top Insights**:
  - **US & Canada** had the highest coverage, followed by **Europe** and **World**.
  - The data highlighted key topics covered by BBC News, providing a clear picture of their focus.

---

## **Project Structure**
```
bbc-news-web-scraping/
├── README.md
├── requirements.txt
├── bbc_news.ipynb
├── bbc_news_world.csv
├── images/
│   ├── top_5_categories_chart.png
└── presentation/
    ├── bbc_news_presentation.pptx
```

- **bbc_news.ipynb**: The Jupyter notebook containing the code for web scraping, data cleaning, and analysis.
- **bbc_news.csv**: The CSV file containing the scraped and cleaned news data.
- **images/**: Contains output images and visualizations.
  - **top_5_categories_chart.png**: A bar chart showing the frequency of the top 5 categories in the data.
- **requirements.txt**: A list of required libraries to run the project.
- **presentation/**: Contains supporting presentation materials.
  - **bbc_news_presentation.pptx**: The PowerPoint presentation that provides an overview of the project, including web scraping process, data analysis, and insights.
