# Project Pivot

### Folder Contents
1. **"Scraping Zillow.ipynb":** Contains the code used to scrape Zillow, generate data visualizations, and perform machine learning modeling and analysis.
1. **"Zillow Scrape 4.10.24":** Contains data collected after a successful scrape of Zillow on April 10, 2024.
1. **"4.10.24 Duplicates Removed":** Contains data that has been cleaned by removing duplicates picked up during the scraping process.

### Reason and Explanation of Change

**TL;DR:**

1. The initial plan was to use Zillow data.
2. Access to Zillow data was denied.
3. The previous dataset appeared to contain fake data, necessitating a switch to real data.
4. Scraped data directly from Zillow's website.

From the start of the project, my goal was to use Zillow data to predict house prices based on available features. However, my application for access to Zillow's API was denied, so I needed an alternative data collection method. For the first two milestones, I used a dataset from Kaggle, but a brief overview suggested it might be fake data. I had not yet found an efficient way to access Zillow's data directly. Currently, I'm taking Dr. Eloe's Web Mining class, where we covered web scraping a few weeks ago. I decided to scrape Zillow's website to gather the data I needed. Consequently, the dataset in this folder now contains fewer features for modeling but is more reliable as it originates directly from Zillow.


### Data Collection

**TL;DR:**
1. Access webpages using the Requests package.
1. Copy page source using Beautiful Soup.
1. Locate the unordered list element with house listings.
1. Extract JavaScript data with the required information, excluding elements with missing values.
1. Parse the required data.
1. Add data to a list.
1. Convert the list to a CSV file.

For data collection, I used the Requests and Beautiful Soup packages to access webpage data and parse it with the JSON package. I iterate through each page in the region being scraped, pausing randomly between 30 and 60 seconds between pages to avoid timeouts. Once I gather the required data, I format it as an array and convert the results to a CSV file. I scraped data from five different areas: Kansas City, MO; Kansas City, KS; Overland Park, KS; Saint Joseph, MO; and Omaha, NE. For each area, I created a new function with the necessary parameters to confine the scraping to the specified area.

### Data Analysis



### Results