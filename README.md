# mars-review

<h2>Instructions</h2>
<h3>Part 1: Scrape Titles and Preview Text from Mars News</h3>
<p>Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.</p>

<ol>
<li>Use automated browsing to visit the Mars news siteLinks to an external site.. Inspect the page to identify which elements to scrape.</li>
<li>Create a Beautiful Soup object and use it to extract text elements from the website.</li>
<li>Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:</li>
    <ul>
    <li>Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. </li>
    <li>Store all the dictionaries in a Python list.</li>
    <li>Print the list in your notebook.</li>
    </ul>
</ol>

<h3>Part 2: Scrape and Analyze Mars Weather Data</h3>
<p>Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.</p>

<ol>
<li>Use automated browsing to visit the <a href="https://static.bc-edx.com/data/web/mars_facts/temperature.html">Mars Temperature Data SiteLinks</a> to an external site.. Inspect the page to identify which elements to scrape.</li>
<li>Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.</li>
<li>Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:
    <ul>
    <li>id: the identification number of a single transmission from the Curiosity rover
    <li>terrestrial_date: the date on Earth
    <li>sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
    <li>ls: the solar longitude
    <li>month: the Martian month
    <li>min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
    <li>pressure: The atmospheric pressure at Curiosity's location
    </ul>
</li>
<li>Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.</li>
<li>Analyze your dataset by using Pandas functions to answer the following questions:
    <ul>
    <li>How many months exist on Mars?</li>
    <li>How many Martian (and not Earth) days worth of data exist in the scraped dataset?</li>
    <li>What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:</li>
        <ul>
        <li>Find the average minimum daily temperature for all of the months.</li>
        <li>Plot the results as a bar chart.</li>
        </ul>
    <li>Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question:</li>
        <ul>
        <li>Find the average daily atmospheric pressure of all the months.</li>
        <li>Plot the results as a bar chart.</li>
        </ul>
    <li>About how many terrestrial (Earth) days exist in a Martian year? To answer this question:</li>
        <ul>
        <li>Consider how many days elapse on Earth in the time that Mars circles the Sun once.</li>
        <li>Visually estimate the result by plotting the daily minimum temperature.</li>
        </ul>
    </ul>
</li>
<li>Export the DataFrame to a CSV file.</li>
</ol>