# RAW_DATA

## Links
[First Dataset](DataSets\Housing.csv)\
[Zillow Scraper](ScrapingZillow.ipynb)\
[Second Dataset](DataSets\ZillowScrape4.10.24.csv)\
[Second Dataset Duplicates Removed](DataSets\4.10.24DuplicatesRemoved.csv)\
[Link to next markdown file DATA.md](DATA.md)

## Data Aquisition
The initial dataset that I used for this project was [Housing.csv](DataSets\Housing.csv) found from [Kaggle](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset/data). I used this dataset for the first two milestones, however after using it and looking at the results I determined that I wasn't going to use it any longer due to the unknown validity of the data.

After deciding to not use my initial dataset I decided that I would web scrape Zillow for data. I made this decision because I am currently in Web Mining and thought that it would be a cool to use the data from one project for another.

### Methodology
My methodology for my data collection was as follows: Use Requests Python package to fetch page data from Zillow, within my request I used a specific parameter for the area I wanted to scrape. I then passed that response into the BeautifulSoup package so that I could parse through it later for data. I used and xml parser to find the elements that contained the data I was looking for. I proceeded to put the collected data into a Python dictonary that was then put into a list. During this process I ignored all house listings that were missing a floor size. I used a loop to change the current page that was being scraped. After I ran the program and collected the data for each city I then exported the results list to a csv.


### Features Gathered
The featues I was able to collect were: price, floor size, longitude, latitude, and URL. The reason for only getting 5 features, only 4 of which were used for data manipulation was due to the limited information present in the Zillow listings page. It may have been possible to open each URL of each house and gather more information but that would have increased the complexity of the project greatly. I also thought that location data and the floor size would be enought to accurately predict the price.

