# CS591 Project 1

## Project Questions to Explore
Is there a correlation between neighborhood demographics and the availability and accessibility to MBTA services in the
Greater Boston Area? Using this information, does the MBTA enable or limit economic opportunity for low-income residents?

## Datasets
### MBTA Developer Portal
We make calls to the MBTA portal using a location and retrieve information on any MBTA stops that fall within a 1 mile radius. The 
locations that we use are longitude and latitude coordinates that span all of the neighborhoods in the Greater Boston Area. 

### U.S. Census Bureau - American Community Surveys
American Community Surveys are helpful in finding detailed information about people and lifestyle within local communities around 
the country. We used four datasets that were collected from the 2010-2014 5-Year American Community Survey and that contain information 
about specific Boston neighborhoods. These datasets cover the following areas: race, poverty, means of commuting, and household income

### GeoData Service
We make calls to this web service using their publicly accessible API. Similarly to the MBTA Developer Portal, we use longitude 
and latitude coordinates as paramaters to retrieve results pertaining to demographics, geography, and lifestyle data. 

### Using the Datasets 
All three of these data sources can be combined in various ways to explore the questions for our project. With the MBTA API, 
we will be able to see how accessible and available public transit is to different locations in Boston. If we were to map all 
of the stops returned by our queries on a map, it would be very interesting to see if some areas were more densely populated with 
stops compared to others. Another layer that we can explore using this data is the problems that the accessibility (or lack thereof) 
to the MBTA causes to communities which rely on public transportation the most.  Are we being fair in our distribution of 
public resources? This is where we will use the information from the ACS the most, as those will inhibit us to see different social 
demographic factors for each neighborhood in Boston. Lastly, the data we collect from the GeoData service can be used to explore 
the effects of any inequality that become apparent in our findings. For example, do we see an increase in vacant houses in locations 
with more employees and less accessibility to public transportation? 

## Project 1 Notes
### Pandas Library
We used the popular data analysis tool for Python, Pandas, to do our data transformations. Pandas is mainly used to find the results 
of taking the union of several datasets. We also use Pandas to aggregate column data to find sums and averages. The library is 
properly imported at the top of our Python files. If there is a need for installation, the command "pip instal pandas" can be run
from the command line. If that doesn't work, see https://pandas.pydata.org/pandas-docs/stable/install.html for more details.