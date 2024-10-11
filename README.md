BBC News Web Scraping Project
Project Overview
This project involves web scraping news articles from the BBC News website to gather headlines, categories, timestamps, and author information. The objective is to collect, organize, and analyze this data for insights, and store it in a structured CSV format for further use.

Objective
Scrape news data from BBC News, including headlines, categories, authors, and publication timestamps.
Organize the data in a well-structured CSV file for ease of analysis and visualization.
Analyze trends, such as the most frequent categories, to understand BBC's focus areas.
Technologies and Tools Used
Programming Language: Python
Libraries:
requests: For sending HTTP requests to retrieve HTML content.
BeautifulSoup: For parsing HTML and extracting relevant data like headlines, categories, etc.
pandas: For organizing extracted data into a DataFrame and exporting it to CSV.
lxml: Used as an HTML parser.
matplotlib: For data visualization (e.g., charts of the top categories).
IDE: Google Colab for executing and developing the code.
Web Scraping Process
Sending HTTP Requests: Used requests to fetch the HTML content from BBC News.
Parsing HTML: Extracted the necessary elements (e.g., headlines, categories) using BeautifulSoup.
Data Cleaning:
Dropped the Author column due to insufficient data.
Converted Timestamp into a date-time format for easy analysis.
Removed rows with missing values in critical columns like Category and Timestamp.
Data Storage: Organized and exported the cleaned data into a CSV file for easy sharing and analysis.
Data Analysis and Visualization
Generated visuals (e.g., bar chart) to showcase the Top 5 News Categories from the scraped data.
Top Insights:
US & Canada had the highest coverage, followed by Europe and World.
The data helped highlight key topics covered by BBC News, providing an overview of their focus.
Project Structure
bbc_news.ipynb: The Jupyter notebook containing the code for web scraping, data cleaning, and analysis.
bbc_news.csv: The CSV file containing the scraped and cleaned news data.
images/: Contains output images and visualizations.
top_5_categories_chart.png: A bar chart showing the frequency of the top 5 categories in the data.
requirements.txt: A list of required libraries to run the project.
