## Final Project: Script 1
### Web-scraping Weather Forecast Information with Python
In Script 1, we put our web-scraping skills to use by scraping the National Weather Service (NWS) page. The goal was to obtain the 5-day weather forecast from any location in the US and rendering the output in capital letters. The script has comment codes but can be broken down in the following simple steps:

- The user is asked to enter a latitude and a longitude of any location in USA. 

- The script concatenates the latitude and longitude to the NWS URL (https://forecast.weather.gov/). At this point one could even check to see if the website exists. 

- Then one could send a request to the NWS website so we can `get()` the URL and obtain information from this page. 

- BeautifulSoup library is used for scarping the NWS page.

- Then one needs to locate the items that must be scraped. The `forecast-tombstone` class in the `li` tag contains the weather forecast information. 

- Since multiple elements are being scraped under the `forecast-tombstone` class a loop is used to obtain all the text that gives information on the weather forecast. 
- To have the right spacing, one can `replace()` the output with a formatted result.
- Finally, one can further use a string manipulation technique to generate the output in uppercase. 

## Final Project: Script 2
### Web-visualization using Plotly
In Script 2, I had the opportunity to use an open-source library which creates interactive charts on Python called **plotly**. I follow a tutorial (https://towardsdatascience.com/how-to-create-a-plotly-visualization-and-embed-it-on-websites-517c1a78568b) to create an interactive chart which shows the life expectancy of the continents in the world given their gross domestic product (GDP) per capita in 2007. This script also has comments but can be broken down in the following simple steps:

- First one should install and import plotly express so that we can display the visualizations in a python notebook. 
- Then one uses data from Gapminder (https://www.gapminder.org/) of the countries in the world in 2007, grouped as continents and weighted by their population. The data is also attached in a CVS file in this repository. 
- To embed the figure created, one must install and import `chart_studio` and create an account in https://chart-studio.plotly.com/.
- Finally one pushes the visualization to chart studio and uses the embed code so this also appears on a website hosted by GitHub pages: https://nayantarab.github.io/Web_Visualization/     
 
The chart shows that life expectancy is an increasing function of GDP per capita. The colors of the circles represent the continents while the size is the population. GDP per capita is one of the many measures to judge the well-being of an economy and is the total income of a country normalized by its population, while the life expectancy is measured in number of years a person lives in a country. By clicking on the figure, a page opens to the interactive diagram which shows that Japan has the highest life expectancy while the Democratic Republic of Congo (DRC) is the lowest. This is expected since an average person’s makes 30,000 local currency units (LCU) more in Japan compared to DRC. 

In the future, I plan on using these tools to build my own website which could be hosted on GitHub pages as well as add my projects on GitHub so that they are accessible to anyone who might be interested in my research. The markdown on GitHub also makes it easy to keep a record of my projects and improve my documentation skills. I definitely see myself using GitHub as well as Python in the near future and I am excited to continue my coding journey and make my work as *open-source* as possible!  
