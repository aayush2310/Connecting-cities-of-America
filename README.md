# Connecting-cities-of-America
Using Dijkstra's algorithm to connect America's biggest cities.   
http://127.0.0.1:5500/C++%20in%20VSCODE/index.html

It's an implementation of Dijkstra's algorithm! The concept is to find the shortest path between cities to get from one to another, for example, if Los Angeles and 
New York City were chosen, lines would be drawn connecting intermediary cities, such that the total line length is minimized. Torender the cities I used a JSON dataset
of the USA's 1000 largest cities by population and I converted theirlongitudinal and latitudinal coordinates to x and y positions using the Mercator projection. Of 
course directlines could not just be drawn between the two chosen cities, instead, to facilitate the path-finding I neededpaths, since I did not have an accompanying
dataset of roads, I had to approximate my own. To do this I createda road between every city that was at or below the average distance between cities. All the 
path-finding willmade use of these roads. A problem this road solution did not account for however was connecting the east andwest coasts, as when there are few cities, 
the sides tend to be isolated, to hopefully compensate for this thereis always a road between LA and NYC. The purpose of this project was to explore advanced algorithms.
