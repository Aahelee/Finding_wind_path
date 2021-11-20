# Finding_wind_path

In this project, the monthly wind path is tracked for any location inside the border of Bangladesh. The wind path can either end at the target point or start from it.

# Data Description

1.The files "10m_u_component_of_wind" and" 10m_v_component_of_wind" contain the eastward and northward components of the wind from the "ERA5 monthly averaged data on pressure levels from 1979 to present" dataset, which is available in https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-pressure-levels-monthly-means?tab=form. 
The datasets are then converted to CSV format. The CSV files are u10 and v10, respectively. But the format of the data NetCDF files often changes on this site. So, if downloaded now, the preprocessing can be different.
2.The excel file "map" contains the points along the perimeter of Bangladesh and its districts.
3.The file "position_densified" contains the points along the Himalayan ridgeline and the Bay of Bengal.


# Project Description

The direction and path of the wind can be a significant factor in the overall climatic condition. For example, during the rainy season in Bangladesh, the monsoon wind carries moisture in this region and causes rainfall. This wind comes from the southeast crossing the coastline of the Bay of Bengal. Here the target area is within 84°-96° E longitude and 19°-28° N latitude. 

After finding the wind path, they are divided into 4 categories, wind that crosses the coastline, the wind that crosses the ridgeline, the wind that gets outside the target area before crossing any of them, and wind that falls into a vortex. The other parameters are the time it takes to reach that location, the distance it travels, and whether it comes from the coastline or the ridgeline of the Himalayans.

The travel path of wind after leaving the location is also generated along with the necessary parameters. 

# Author

Aahelee Sarker (aahelee.sarker@gmail.com)

# Acknowledgments

code snippets are taken from  these sites:

1.<a href="https://nathanrooy.github.io/posts/2016-09-07/haversine-with-python/#%20y1%20=%20latitudes">Calculating the Distance Between Two GPS Coordinates with Python (Haversine Formula)</a> <br>
2.<a href="https://bryceboe.com/2006/10/23/line-segment-intersection-algorithm/">Line Segment Intersection Algorithm</a> <br>
3.<a href="http://paulbourke.net/geometry/pointlineplane/javascript.txt">intercepting point</a>
