### Pa. DDAP inspection scraper - select providers

Python script built with Scrapy to scrape inspections for specific facilities from Pa. Department of Drug and Alcohol
 Programs website. This program is a companion to [ddap_scraper](https://github.com/SimmonsRitchie/ddap_scraper
 ), which scrapes _ALL_ facilities available on the DDAP website rather than specific providers.

#### Requirements

- Python 3.6+

#### Install

1. Open the terminal. Clone the project repo:

    `git clone https://github.com/SimmonsRitchie/ddap_scraper_select.git`

2. If you don't have pipenv installed on your machine, run:

    `pip install pipenv`

3. Navigate into the project directory:

    `cd ddap_scraper_select`
     
4. Use pipenv to create a virtual environment and install the project 
dependencies. Run:

    `pipenv install`

5. Update 'facility_list.csv' in ddap/ddap/input

#### Run

This project uses Scrapy and takes advantage of its excellent CLI.

In the terminal, navigate to the project's root directory and then into the ddap directory:

`cd ddap`

To begin the scrape and generate a CSV of scraped data, run:

`scrapy crawl inspections -o scraped_data.csv`

To generate a JSON or XML file, just swap the file extension. Eg.

`scrapy crawl inspections -o scraped_data.json`

