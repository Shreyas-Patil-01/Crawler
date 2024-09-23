# SCRAWLER
## Newspaper Scraping Using Scrapy

This repository contains a web scraping tool built using Scrapy to scrape news articles from the Livemint website. It extracts article URLs, titles, author details, content and published dates and stores the data in a JSON file.

## Table of Contents
- [Project Overview](#project-overview)
- [Workflow](#workflow)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Example Output](#example-output)
- [Contributing](#contributing)
- [License](#license)
- [Notes](#notes)

## Project Overview

### Description
This project uses Scrapy to scrape news articles from Livemint. It follows category links on the homepage and scrapes details such as the article title, author, content, and published date from each article. The scraped data is stored in a JSON file (`articles.json`).

### Features
- Scrapes news articles from **Livemint**.
- Extracts key details such as **article URL**, **title**, **author name**, **author URL**, **article content**, and **published date**.
- Saves scraped data in a **JSON** format.
- Implements a delay between requests to avoid overwhelming the server.

## Workflow

Below is the visual workflow of the Scrapy process for scraping the news articles:

![Scrapy Workflow](https://github.com/Shreyas-Patil-01/Scrawler/blob/main/News_scraper/WorkFlow.png)

This diagram outlines the steps from starting with the homepage, following category links, parsing articles, and saving them to a JSON file.

## Installation

### Prerequisites
Make sure you have Python 3.x and Scrapy installed. You can install Scrapy via pip:

```bash
pip install scrapy
git clone https://github.com/Shreyas-Patil-01/Scrawler.git
cd Scrawler
scrapy runspider spider.py
```

## Project Structure
.
├── spider.py            # The main Scrapy spider file
├── articles.json        # Output file where scraped data is stored
├── workflow_image.png   # Workflow diagram image
└── README.md            # This README file

## Example Output
{
  "article_url": "https://www.livemint.com/some-article",
  "title": "Some Article Title",
  "author_name": "John Doe",
  "author_url": "https://www.livemint.com/authors/john-doe",
  "article_content": "This is the content of the article...",
  "published_date": "20 Sep 2024"
}

![Scawler_running_output](https://github.com/Shreyas-Patil-01/Scrawler/blob/main/Output.png)

## Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

-Fork the repository.
-Create a new feature branch.
-Commit your changes.
-Push to the branch.
-Open a pull request.

Feel free to open issues or submit pull requests for improving the scraper or adding new features.
