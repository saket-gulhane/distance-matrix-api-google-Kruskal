# distance-matrix-api-google-Kruskal
Find minimum cost spanning tree on "n" cities, whose distance is calculated using Google Distance Matrix API.


## Inputs to be provided:  
  1. List of citites (file: "./inputs/cities.txt).
  2. List of pair of cities, whose edges has to be excluded to find spanning tree (file: "./inputs/remove.txt").  
  
  ![alt text](https://user-images.githubusercontent.com/47126380/67140243-6240fe00-f276-11e9-9df6-3ae0db66427a.png)
  Input in "cities.txt" must be of format "indexNumber cityName" each on a new Line. Where indexNUmber starts from 0.

  Input in "remove.txt" must be of format "cityA cityB", where both city names are seperated by a space.
  

## Output:
  1. List of "n-1" edges forming minimum cost spanning tree.
  2. Cost of spanning tree.
  
  ![alt text](https://user-images.githubusercontent.com/47126380/67140312-f3b07000-f276-11e9-8009-eb6993d7678a.png)
  
  
  
## Description of python program:
  Algorithm used: Kruskal algorithm to find minimum cost spanning tree.
  "daaf.py": Used to geneate all possible edges and find the distance using Google Distance API between input cities, excluding edges given              as input in "./inputs/remove.txt" file.
  To get your own Google API key: [click here](https://cloud.google.com/maps-platform/)
  "edgesList.txt": Store edges and distance between 2 cities.
  
  "kruskal.py": Calculate the minimum cost spanning tree generated and store result in "./output/output.txt"
  

## Reference:
   1. kruskal algorith: [https://en.wikipedia.org/wiki/Kruskal%27s_algorithm](https://en.wikipedia.org/wiki/Kruskal%27s_algorithm)
   2. Google API key Generation: [click](https://cloud.google.com/maps-platform/)
