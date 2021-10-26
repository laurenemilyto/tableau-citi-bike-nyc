![Dashboard](https://i.pinimg.com/originals/8d/1e/18/8d1e18d24c94e1b3fdf432796a6f1b21.jpg)

## Background
Citi Bike is a privately owned public bicycle sharing system serving the New York City boroughs of the Bronx, Brooklyn, Manhattan, and Queens, as well as Jersey City, New Jersey, and Hoboken, New Jersey. 

For this project, I analyzed potential changes to the Citi Bike NYC program for city officials looking at pre-Covid months May, June, July in 2019 and respective months in 2020 during Covid. Data was cleaned via Jupyter Notebook in Python/Pandas and 

Citi Bike Covid Story: [Link](https://public.tableau.com/app/profile/lauren.to8058/viz/CitiBikeCovidAnalysis/CitiBikeStory?publish=yes)

## Technology
- Pandas
- Geopy
- Python
- Tableau Desktop

## Process
Data was imported from six csv files into Jupyter Notebook, merged, cleaned, and extracted into a single csv file (2M KB). Using Python/Pandas the following transformations were performed: 

Transformations
- Concatenated six csv files
- Removed null values
- Dropped unnecessary columns
- Dropped rides where duration < 300 secs (or 5 min)
- Dropped rides where duration > 24 hours
- Dropped rides where start and end station are the same
- Modified column data types to 'int'
- Added ride_id column to identify each ride
- Added distance(mi) column using Geopy
- Divided riders into bins by birth year and appended to age column

## Analysis
The focus of this analysis is to compare changes in the Citi Bike program pre-Covid and during Covid, assessing user types and age. 

- Riders rode an average of .3 miles farther in 2020 during the pandemic than in 2019. Average distance riden increased across every age group. However, riders in the 19-29 year old bracket, along with riders in the 30-39 year old bracket covered the most distance and had the largest distance increase (.3 miles). 

- 30-39 year olds are Citi Bike power users. They took the most rides in May, June and July of 2019 (~1.7M), but rides dropped (~1.5M) in 2020 during the pandemic. Overall, the total number of rides dropped by 500K from 2019 to 2020 across the city. 

- Rides decreased in 2020, and so did subscribers. 2020 saw 10% fewer subscribers than 2019.  

- Riding increases seasonally in the summmer as the weather gets warmer. Out of months analyzed: May, June and July, you can see rides steadily increasing, peaking in July with ~1.7M riders both years.

- In 2019, Tuesday and Wednesday were the most popular days to use a Citi Bike from 5pm-6pm, likely commuters heading home from work. However in 2020, Sunday was the most popular day to use a Citi Bike from 1pm - 6pm. This indicates a switch to locals using the Citi Bike system from commuting to leisure during the pandemic.

- Overall, men take about double the amount of Citi Bike rides as women. However, men were less likely to ride a Citi Bike in 2020 (down 800K rides from 2019), while women were more likely to ride a Citi Bike in 2020 (up 200k from 2019).

- 12 Ave & W 40 St (Lincoln Tunnel), and West St & Chambers St (Tribeca) remained the most popular start and end stations. A noticeable change from 2019 to 2020 is that rides from Pershing Square North station (by Grand Central Terminal) greatly decreased, perhaps due to fewer people arriving/commuting in NY via train due to the pandemic. 


## Data Source
[Citi Bike Program Data](https://ride.citibikenyc.com/system-data)

## Contact
Lauren To: [laurenemilyto@gmail.com](laurenemilyto@gmail.com)
