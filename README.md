# Surfs Up: A Climate Analysis of Oahu, Hawaii

## Overview of the Analysis

The purpose of this analysis was to help W. Avy determine if opening a surf and ice cream shop is a sustainable, year-round business. To help him, I analyzed temperature trends in Oahu, Hawaii during the months of June and December. To accomplish this, I queried Hawaii weather station data. If the weather is warm and doesn't vary too much during either of those months, W. Avy's should move forward with the business idea, and if not, he should proceeed with caution. Here's what I found.  

## Results of the Analysis

### Analysis Resources
* Data Sources: [Hawaii_Weather_Data](https://github.com/dwwatson1/surfs_up/blob/main/hawaii.sqlite)
* Software: Jupyter Notebook 6.1.4, VS Code 1.55.0, SQLAlchemy
* Notebooks: [climate_analysis](https://github.com/dwwatson1/surfs_up/blob/main/climate_analysis.ipynb) & [SurfsUp_Challenge](https://github.com/dwwatson1/surfs_up/blob/main/SurfsUp_Challenge.ipynb)
 
### Overview of Results 
To complete my climate analysis, I ran two queries to obtain all June and December temperatures from Oahu weather station data and store them in lists. Then, I converted the lists into a Dataframe using Pandas. Using the .describe() function. 

#### June Temperature Summary
<img src="https://github.com/dwwatson1/surfs_up/blob/main/June_Temps.png" width="250" >

#### December Temperature Summary
![December_Temps](https://github.com/dwwatson1/surfs_up/blob/main/December_Temps.png | width=100)

#### Takeaways from Temperature Data
The temperature summary statistics from June and December for the island of Oahu are shown above. This weather data comes from 9 different stations dating back to 2010, which accounts for the many [micro climates](https://www.to-hawaii.com/oahu/weather.php) on the island itself. 

- Temperatures are fairly uniform year-round. The average temperature difference between June (75 degrees) and December (71 degrees). For including max and min temperatures, that's quite warm, but not uncomfortably hot.
- The standard deviation in December is slightly higher than June (3.75 vs. 3.26), which shows that there is more temperature variance in December, albeit minimal. This data also confirms that the temperatures don't fluctuate much.
- The minimum temperatures between June and December show that greatest difference of 8 degrees (64 vs. 56 degrees). While 56 may be chilly for Hawaii standards, I'm sure Californians would say that weather is more than suitable for surfing and ice cream consumption. 

### Summary
From this climate analysis, we determined that the temperatures in Oahu are steadily warm. The temperatures in June and December never go above 85 or below 56. Year-round warm temperatures are ideal for tourism and locals getting outside to either surf or eat ice cream. I recommend W. Avy move forward with opening up his shop. But, before moving forward, I recommend W. Avy consider two more data points.

#### Additional Queries
To figure out when it's most ideal to surf, we need to look at wind speeds as this likely affects surf height. We should also query surf height as this is a metric the [National Weather Service](https://www.weather.gov/hfo/surfreports) tracks on the Hawaiian islands. Doing so would confirm the two are related. The wind and surf height will tell us if wind and surf height changes based on seasons. Surfers tend to like big waves, so any insight into the surf height metric may show when surfers congregate in Oahu.

I also recommend querying ocean temperatures. The warmer the ocean temperatures are, the more likely surfers and beachgoers will be around the water. [This website](https://www.to-hawaii.com/oahu/weather.php) notes that the average ocean temperature in Oahu in February is 75 and 80 in September. With this information and more from a future query, we're likely to find that like air temperature, ocean temperatures don't change much. This is warm enough to swim and surf year-round. 
