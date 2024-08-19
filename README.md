# Web scraping challenge

## Background
You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.

As you work on this Challenge, remember that you’re strengthening the same core skills that you’ve been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating your insights.

## What You're Creating
This new assignment consists of two technical products. You will submit the following deliverables:

* Deliverable 1: Scrape titles and preview text from Mars news articles.

* Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

### Files
Download the files to help you get started in thhe resources folder.

## Instructions
### **Part 1: Scrape Titles and Preview Text from Mars News**

* Open the Jupyter Notebook in the starter code folder named **part_1_mars_news.ipynb.** You will work in this code as you follow the steps below to scrape the Mars News website.

* Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.

**hint: To identify which elements to scrape, you might want to inspect the page by using Chrome DevTools to discover whether the table contains usable classes.**

1. Create a Beautiful Soup object and use it to extract text elements from the website.

2. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

3. Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. An example is the following:

  *{'title': "NASA's MAVEN Observes Martian Light Show Caused by Major Solar Storm",
 'preview': "For the first time in its eight years orbiting Mars, NASA’s MAVEN mission witnessed two different types of ultraviolet aurorae simultaneously, the result of solar storms that began on Aug. 27."}*

* Store all the dictionaries in a Python list.

* Print the list in your notebook.

4. Optionally, store the scraped data in a file (to ease sharing the data with others). To do so, export the scraped data to a JSON file. (Note: there will be no extra points for completing this.)




## **Part 2: Scrape and Analyze Mars Weather Data**

1. Open the Jupyter Notebook in the starter code folder named **part_2_mars_weather.ipynb.** You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

2. Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site. Inspect the page to identify which elements to scrape. Note that the URL is **https://static.bc-edx.com/data/web/mars_facts/temperature.html.**

**hint: Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.**

3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

* **id:** the identification number of a single transmission from the Curiosity rover
* **terrestrial_date:** the date on Earth
* **sol:** the number of elapsed sols (Martian days) since Curiosity landed on Mars
* **ls:** the solar longitude
* **month:** the Martian month
* **min_temp:** the minimum temperature, in Celsius, of a single Martian day (sol)
* **pressure:** The atmospheric pressure at Curiosity's location.
  
4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

**hint: You can use the Pandas astype and to_datetime methods to accomplish this task.**

5. Analyze your dataset by using Pandas functions to answer the following questions:

* How many months exist on Mars?
* How many Martian (and not Earth) days worth of data exist in the scraped dataset?
* What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
* Find the average minimum daily temperature for all of the months.
* Plot the results as a bar chart.
* Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
* Find the average daily atmospheric pressure of all the months.
* Plot the results as a bar chart.
* About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
* Consider how many days elapse on Earth in the time that Mars circles the Sun once.
* Visually estimate the result by plotting the daily minimum temperature.
* Export the DataFrame to a CSV file.

## References
The Mars News websiteLinks to an external site. is operated by edX Boot Camps LLC for educational purposes only. The news article titles, summaries, dates, and images were scraped from NASA's Mars NewsLinks to an external site. website in November 2022. Images are used according to the JPL Image Use PolicyLinks to an external site., courtesy NASA/JPL-Caltech.

![Mars planet](Resources/28e52c71c91e8fc3f4678a64f6bc0dfe.jpg)
