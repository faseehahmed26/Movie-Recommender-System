# Bollywood Movies Recommender System

![Movies](https://user-images.githubusercontent.com/54709992/172464455-e51c415b-ed6c-49ae-909a-8585c7542170.png)

## Overview

A data collection and processing pipeline that extracts information from IMDB for 3,100+ Bollywood movies to build a recommendation system. This project uses web scraping techniques to gather comprehensive movie metadata that serves as the foundation for content-based movie recommendations.

## Features

- **Web Scraping**: Automated extraction of movie data using BeautifulSoup and Requests
- **Data Collection**: Retrieval of movie titles, cast, plot summaries, release dates, genres, and reviews
- **Data Processing**: Cleaning and structuring raw HTML data into analysis-ready formats
- **Feature Engineering**: Creation of derived metrics like content age and metadata analysis
- **ETL Pipeline**: Complete extract, transform, and load workflow for movie data

## Technologies

- Python
- BeautifulSoup
- Pandas
- Requests
- HTML/CSS parsing
- Data cleaning techniques
- ETL methodologies

## Dataset

The processed dataset includes 11 features for 3,123 Bollywood movies:
- Title and IMDB ID
- Cast information
- Plot summaries and keywords
- Genre classification
- Release date and year
- Content age (years since release)
- Duration
- Reviews

## Pipeline Structure

1. **Search Query Generation**: Convert movie titles to IMDB search URLs
2. **Main Link Extraction**: Extract specific movie page links from search results
3. **Content Scraping**: Retrieve detailed information from individual movie pages
4. **Data Transformation**: Clean and structure raw scraped content
5. **Feature Engineering**: Calculate additional metrics from base data
6. **Data Storage**: Export processed data to CSV for the recommendation engine

## Future Work

- Implement sentiment analysis on movie reviews
- Calculate cast and crew popularity scores
- Develop content-based recommendation algorithms
- Create similarity metrics based on plot keywords and genres
- Build a user interface for movie recommendations

## Usage

```python
# Install required packages
pip install -r requirements.txt

# Run the scraper
python movie_scraper.py

# Process and analyze data
python data_processor.py
