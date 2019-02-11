# The Battle of the Neighborhoods

This capstone project was completed as a course requirement for the IBM Data Science Professional Certificate Specialization on Coursera.

# Introduction

Toronto is the capital city of the province of Ontario and the largest city in Canada by population. The economy of Toronto is the largest contributor to the Canadian economy. Many IT companies have their offices in Toronto.

A fictional IT company based in Rosedale, Toronto needs to choose a location and a possible list of hotels for their employees who will be traveling to Melbourne for few weeks to work at their client office in Melbourne, Australia. Melbourne is one of the largest cities in Australia, with an area of 9,992.5 km2 covering 31 municipalities and over 345 localities. The company would like to choose only from those locations in Melbourne which are similar to Rosedale for their employees’ accommodation in order to make them feel more comfortable and help them to adapt quickly to the new place. In this project we will attempt to help the company find those locations in Melbourne which are similar to their own location in Rosedale, Ontario.

• Therefore, the problem to be answered is:  “Which areas of Melbourne are similar to Rosedale, Ontario? Can we have the names and locations of hotels in these locations where accommodation can be arranged for their employees?”

• Who would be interested in this project?: In this project I attempt to help a fictional IT company in Toronto choose a locality which is similar to theirs. Anyone wishing to compare neighbourhoods similarly can check out this analysis.

# Project Description

The data that we have used in this project is obtained from Wikipedia and Foursquare. We have obtained the list of localities or neighbourhoods of Toronto and Melbourne from the following Wikipedia pages and website, as well as their geo-location data like latitude and longitude.

https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

https://en.wikipedia.org/wiki/Postal_district_numbers_of_Melbourne

http://www.mapdevelopers.com/batch_geocode_tool.php

These data is then scraped using the Beautiful Soup library in python, and then formatted into a pandas dataframe  for further processing. 

Foursquare provides detailed data relating to each of these neighbourhoods. Foursquare is a local search-and-discovery service mobile app which provides search results for its users. Foursquare API will be used to explore the various types of venues and their categories available in each neighborhood. The information for venues, categories, hotels, etc is extracted using foursquare to solve the business problem. This data is to be used for segmenting and clustering the localities of Melbourne, on the basis of their shared characteristics and features.

The k-means clustering algorithm is employed to perform this task. The sklearn.cluster package from the sci-kit library is used for performing the clustering.This will help to detect the similarities and dissimilarities of neighborhoods. We find the cluster which is most similar to Rosedale and then obtain a list of some of the hotels which are located in this. Finally, the Folium library is utilized to visualize the neighborhoods in Melbourne and their clusters. 
 cluster. 


# Technologies Used

Python

Libraries: pandas, numpy, requests, folium

Jupyter Notebook

# Results

The analysis described above was performed and the following cluster of neighbourhoods in Melbourne was obtained that is predicted to show similar features to the original neighbourhood of Rosedale, Toronto. Then a list of five hotels in the selected cluster was obtained using the Foursquare API. This project can be replicated for different neighbourhoods and cities in order to find similar neighbourhoods, and this can be expanded further using different datasets and taking more factors into consideration to provide more accurate analysis.




