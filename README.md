# Global Landslide Catalog Analysis
The landslide data was obtained from [NASA]('https://data.nasa.gov/Earth-Science/Global-Landslide-Catalog-Export/dd9e-wu2v').
The earthquake data was obtained from [USGS]('https://earthquake.usgs.gov/earthquakes/search/')
The rainfall data was obtained from [NEO]('https://earthobservatory.nasa.gov/global-maps/GPM_3IMERGM')

# Analysis
## Objective
This project was created to compare Landslide data that was collected by NASA using News from around the world with Earthquake data, from the USGS, and rain data also from NASA, to see if there are correlation between those events.

## Technical
Using JupyterLab with its Python kernel, I wrote a code to plot the collected data from .xlsx and .csv (both within the folder [Data]('Data')) in a coastline basemap using the Basemap, Matplotlib and Seaborn libraries.
I also created a topographic map to see mountainous regions and link them with the landslide events.
The projection used was the Cylinder and I chose to use Geographic (Degrees and Minutes) instead of UTM (Universal Transversal Mercator) because it polutes less and it is simpler to understand.

## The Data
First step, as said before, was plotting the Landslide data to a basemap to see where those geological events were occuring. The image was the result:

![Landslide Plots](Images/landslide_map.jpg 'Landslides')

From this image alone we can see greater occurencies within the Andes Mountain Range, The Himalain Mountains (Southwest of China) and the Eastern and Western areas of the USA.

We can use the topographic map below to have a better look at mountain ranges (the regions represented by the light brown color, the green areas are less inclined terrain)

![Topographic Map](Images/topographic_map.jpg 'Topographic Map')

Now let's have a look at the Earthquake occurencies and the precipatation:

![Earthquake Plots](Images/earthquake_map.jpg 'Earthquake')

Rainfall map:

![Rainfall](Data/rain_data.jpg 'Rainfall')

Comparing the Landslide Map with the Earthquake, we can see a correlation between those two occurencies within the Andes, Himalain, South Asia/North Oceania, Japan, Italy and Southeastern Europe. Geological events can cause landslides depending on the magnitude of the earthquake, those shown on the map go from 5 to 8 point in the Richter Scale. These are quite powerful and are easily felt from the surface.

But, if not linked to earthquakes, why landslides occur?

Sometimes, the soil gets supersaturated with water from heavy rain and becomes unstable, if the combination of the declination and the water saturated soil are enough, the land starts to move downhill. And here we can add the third map of the global rainfall.
That map indicate to us the why zones like West Africa and the coast of Brazil have so many occurencies (the more blue the color is, the higher the precipitation).

## A Look By the Years
By faceting the plots shown above (landslides and earthquake) I was able to create the occurencies of those events by year, as shown below:

Landslides by year:

![Landslides by year](Images/landslide_facet.jpg 'Landslides by year')

Earthquakes by year:

![Earthquakes by year](Images/earthquake_facet.jpg 'Earthquake by year')

Comparing both graphs we can see the same pattern of landslides occurencies by the years with less occurencies at 2015, this could be explained by the reduction of notifications and/or the events itself.
In 2014 there is a high occurency of landslides at the coas of Brazil, but as shown before, this is due to high volume of rain and, looking again at the topographic map, the elevated terrain.
The same can be seen at southeastern Australia, where the high precipitation and elevated terrain can cause a increase in landslide occurencies.

## In Conclusion
Landslide events can be linked to earthquakes and the result can be catastrophic, one of the greatest examples of this is [Mount St. Helen]('https://youtu.be/UNlP9TGZOMI?t=78'), where in 1980 a earthquake hit the mountain and caused a lateral eruption that chained into the biggets landslide ever recorded.

But, even with a advanced technology it is hard to predict this kind of event.

Landslides by heavy rain are more common and can be avoided by increasing population awareness of dangerous areas as well as the providence of better housing for the people. In Brazil, for example, the housing complexes of the "Favelas" are annualy hit by landslides, many of them with the loss of life, this is due to them being in a very dangerous area and having bad infrastructure.

Taking a look at Africa, there aren't many reported landslides events, just some at the central-eastern area, which is a geological active area and it is better monitored, meaning that those events are happening but they are not being notified.

For Europe, most of the events concentrate in the North Mediterranean, near Italy, which is another geological active area.

In general, most of the data is concentrated within the USA and Eastern Asia, being due to NASA/USGS location in the United States and high occurencies in China.