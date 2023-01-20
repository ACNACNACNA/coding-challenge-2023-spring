# ACM Research coding challenge (Spring 2023)

![image](https://user-images.githubusercontent.com/72369124/211179527-0ee60624-2794-4e13-bf7f-f88b5c950e44.png)

##Summary of the Problem

The dataset given consisted of information about 240 stars. Each star had 7 attributes. Given that there was not a lot of room for inferences within the dataset, I decided to look outward and look into which types of stars would be the most suitable for life. I tested NASA’s observations of K-stars being the best star’s for life using the following parameters: star temperature (in Kelvin), magnitude, spectral class, and the upper/lower bounds of the star’s habitable zone in astronomical units (measured by luminosity).

## Analyzing the Data

First, I got the data of the respective columns, turning the dataframe into a list for easier use. Second, I sorted the data by spectral class using individual lists for each parameter and creating a 2D array for each parameter with the lists within the array representing a specific spectral class. 

To find out what type of star would be the best for life, I looked at the size of the upper bound (since according to the formula, would mean a higher margin between the upper and lower bound of the star’s habitable zone), the proportion of the magnitude compared to the lower bound in order to measure how bright the star would look compared to the Sun’s brightness on Earth, and the proportion of temperature compared to the lower bound in order to see if the temperature in the zone would be similar to Earth’s.

Using matplotlib, I created violin plots of all the parameters, as well as the three metrics I mentioned above to analyze the data. With the last 2 metrics, I normalized them in order to graph the ratio of the star’s metrics and the Sun to the Earth’s.

## Conclusions

	Because G stars only had one data point, I was not able to make any reliable conclusions with their sample size. The K stars’ sample size was not statistically significant either; however, none of the star’s had extraordinarily high magnitudes or temperatures compared to the other stars, suggesting that if one was in the habitable zone of K star’s, the conditions would be similar to Earth. Although the bounds of the habitable zone of K - stars varied, I was not able to prove that K-stars were not the best type of stars for life due to all the other stars being either varied or extraordinarily high compared to Earth.

	In the future, if I was given more time and more data, I would test which star types would suit life the best as well as other star classifications. I would also use more parameters and use more metrics as well as ones more proven to be better metrics, since the metrics I used were more theoretical.


## Sources I used:

https://exoplanets.nasa.gov/search-for-life/habitable-zone/

https://www.bbvaopenmind.com/en/science/physics/planetary-systems-and-the-habitable-zone/#:~:text=In%20order%20to%20calculate%20the,factors%200.95%20and%201.37%2C%20respectively. - the formula for the bounds of habitable life

https://matplotlib.org/stable/index.html - graphing

https://pandas.pydata.org/docs/reference/index.html - pandas

