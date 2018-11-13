# Aggregate polygons by minimum size

The proposed Python code allows to aggregate small polygons with the neighbors, until no polygons remains under a user-define size (area) threshold. The polygon under process is merge with its neighboring polygon that share the longest border.

The script allow for merging shapefile of population data, for example, since the values of the attribute table are summed during the process. The identification of polygons to be processed is based on the area but the user could be easily adapt the code to change this criteria to another (e.g., the perimeter). If the aim is just to aggregate polygons without aggregating any value coming from the attribute table, it should be possible for the user to adapt the code easily. 

As presented here, the user has to provide one polygon shapefile as input with an attribute table containing the population count for each administrative units. 

The code is provided in a Jupyter notebook that allow to run it step by step, giving more ease to the user for adapting to its own data.

## Illustration
![ ](Illustrations/illustration.gif)

## Dependencies
This code mainly relies on [GeoPandas](http://geopandas.org/) and [Fiona](https://pypi.org/project/Fiona/).

- [pandas](https://pandas.pydata.org/)
- [geopandas](http://geopandas.org/)
- [matplotlib](https://matplotlib.org/)
- [numpy](http://www.numpy.org/)
- [seaborn](https://seaborn.pydata.org/)
- [shapely](https://pypi.org/project/Shapely/)