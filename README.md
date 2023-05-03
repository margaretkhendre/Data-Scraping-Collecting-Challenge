# Data-Scraping-Collecting-Challenge

### What You're Creating
This new assignment consists of two technical products. You will submit the following deliverables:

- Deliverable 1: Scrape titles and preview text from Mars news articles.

- Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

## Instructions
### Part 1: Scrape Titles and Preview Text from Mars News
Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.

1. Use automated browsing to visit the [Mars news site](https://static.bc-edx.com/data/web/mars_news/index.html). Inspect the page to identify which elements to scrape.

2. Create a Beautiful Soup object and use it to extract text elements from the website.

3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:

  - Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. 
  
  - Store all the dictionaries in a Python list.
  
  <img width="660" alt="Screenshot 2023-05-03 at 2 19 38 PM" src="https://user-images.githubusercontent.com/121995835/236008489-353b4a59-8ca4-4aab-8b3c-71b26bde5183.png">
  
  - Print the list in your notebook.

### Part 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

1. Use automated browsing to visit the [Mars Temperature Data Site](https://static.bc-edx.com/data/web/mars_facts/temperature.html). Inspect the page to identify which elements to scrape.

<img width="574" alt="Screenshot 2023-05-03 at 4 13 48 PM" src="https://user-images.githubusercontent.com/121995835/236038505-67dfbc40-ccaa-4250-966e-058b5950e9a0.png">

2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.

<img width="574" alt="Screenshot 2023-05-03 at 4 14 23 PM" src="https://user-images.githubusercontent.com/121995835/236038676-fd8f4afa-fb4d-46ea-8308-f6f84c2c1d32.png">

3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

    - id: the identification number of a single transmission from the Curiosity rover
    - terrestrial_date: the date on Earth
    - sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    - ls: the solar longitude
    - month: the Martian month
    - min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    - pressure: The atmospheric pressure at Curiosity's location
    
<img width="574" alt="Screenshot 2023-05-03 at 4 14 51 PM" src="https://user-images.githubusercontent.com/121995835/236038849-88376c70-6e17-4205-af27-e565799f12e8.png">

4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

<img width="772" alt="Screenshot 2023-05-03 at 4 15 54 PM" src="https://user-images.githubusercontent.com/121995835/236039273-d752b854-9545-4628-954f-a71fc945a637.png">

5. Analyze your dataset by using Pandas functions to answer the following questions:

    - How many months exist on Mars? *Refer to jupyter notebook*
    - How many Martian (and not Earth) days worth of data exist in the scraped dataset? *Refer to jupyter notebook*
    - What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:
        - Find the average minimum daily temperature for all of the months.
        - Plot the results as a bar chart.
        
        <img width="627" alt="Screenshot 2023-05-03 at 4 17 18 PM" src="https://user-images.githubusercontent.com/121995835/236039831-fc9d6f43-a567-43d9-8f3b-bab8185002a9.png">

    - Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:
        - Find the average daily atmospheric pressure of all the months.
        - Plot the results as a bar chart.
        
        <img width="627" alt="Screenshot 2023-05-03 at 4 19 10 PM" src="https://user-images.githubusercontent.com/121995835/236040235-cdd52370-95a3-446c-b51a-879b3bbd733e.png">
        
    - About how many terrestrial (Earth) days exist in a Martian year? To answer this question:
        - Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        - Visually estimate the result by plotting the daily minimum temperature.
        
<img width="627" alt="Screenshot 2023-05-03 at 4 19 32 PM" src="https://user-images.githubusercontent.com/121995835/236040319-a808c4dd-8add-4c36-8546-3a6257799c34.png">


