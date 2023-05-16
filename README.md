# Global Landslide Catalog Analysis
The landslide data was obtained from [NASA]('https://data.nasa.gov/Earth-Science/Global-Landslide-Catalog-Export/dd9e-wu2v').
The earthquake data was obtained from [USGS]('https://earthquake.usgs.gov/earthquakes/search/')
The rainfall data was obtained from [NEO]('https://earthobservatory.nasa.gov/global-maps/GPM_3IMERGM')

### Project
- Make a scatter map of the landslides
- Compare with earthquake and rain data

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

Now let's have a look at the Earthquake occurencies and the precipatation:

![Earthquake Plots](Images/earthquake_map.jpg 'Earthquake')

![Rainfall](Data/rain_data.jpg 'Rainfall')

Comparing the Landslide Map with the Earthquake, we can see a correlation between those two occurencies within the Andes, Himalain, South Asia/North Oceania, Japan, Italy and Southeastern Europe. Geological events can cause landslides depending on the magnitude of the earthquake, those shown on the map go from 5 to 8 point in the Richter Scale. These are quite powerful and are easily felt from the surface.

But, if not linked to earthquakes, why landslides occur?

Sometimes, the soil gets supersaturated with water from heavy rain and becomes unstable, if the combination of the declination and the water saturated soil are enough, the land starts to move downhill. And here we can add the third map of the global rainfall.
That map indicate to us the why zones like West Africa and the coast of Brazil have so many occurencies (the more blue the color is, the higher the precipitation).
