## Reference & Resources for Doing Stuff in QGIS

QGIS offers many different functions for creating, managing, editing, and visualizing geospatial data.   

I tend to prefer written resources, so that's what you'll find here.  
But some people prefer videos -- if that's you, search YouTube for whatever task you need help with. There are lots of good QGIS YouTube channels!

### Official QGIS Documentation  

* [QGIS Training Manual](https://docs.qgis.org/3.22/en/docs/training_manual/index.html)  
A great place to start. All the basics presented in a step-by-step manner. 

* [QGIS Desktop User Guide](https://docs.qgis.org/3.22/en/docs/user_manual/index.html)  
Good general reference for all the QGIS functionalities.  

* [A Gentle Introduction to GIS](https://docs.qgis.org/3.22/en/docs/gentle_gis_introduction/index.html)  
A reference for GIS concepts, such as, What's vector data? How do geographic data and attribute data interact? What are methods of visualizing different kinds of geographic data?  

Note that the QGIS documentation is available in **multiple languages, including Russian, French, and simplified Chinese.**  
Click "QGIS Documentation v: 3.22" in the lower-left corner of any of the above pages to see the language options.  

### Useful Tutorials  

* [QGIS Tutorials and Tips](https://www.qgistutorials.com/en/#)  
Ujuval Gandhi has been maintaining and updating this collection of tutorials for a long time, and I really love them.  

### Getting Data from Open Street Map.  

[Open Street Map](https://www.openstreetmap.org) (OSM) is a digital web map of the world that anyone can add data to and extract data from -- kind of a cross beween Google Maps and Wikipedia. Any features that you find on this map can be exported, downloaded, and added as a layer to your QGIS Project.  

OSM has a very active global user community and is a quality source of many types of data (boundaries, cities, roads, rivers, and many, many more).  

Data in OSM is organized by a complex taxonomy of keys (categories), values (sub-categories), and tags (sub-sub-categories). Browse keys and values on this page in the [OSM Wiki](https://wiki.openstreetmap.org/wiki/Map_features). 

Use a tool called [Overpass Turbo](https://overpass-turbo.eu/) to extract data. Here is a sample workflow:  
  1. In the map window, zoom/pan to your region of interest.  
  2. Click the “Wizard” button toward the top of the page.
  3. In the box that pops up, type any key/value or value/tag pair. For example: "amenity=library." (Be aware of the potential size of the dataset that you attempt to extract. For a search like "military=nuclear_explosion_site," it's fine to search the whole globe at once. But if you're searching for libraries, you'll want to restrict the search to a smaller geographic area at a time, or the request will time out before completing.)
  4. Click “Build and run query”
  5. You’ll get a map showing the data that you've extracted. If you want to examine the attributes, click “Data” in the upper-right corner to see a list, or click on locations on the map to examine attributes one-by-one.
  6. Click “Export” in the upper-left.
  7. Next to the word GeoJSON, click “Download” and Save it wherever on your machine you want to.
 
Now you have a GeoJSON file on your computer that you can add to QGIS just like you did with the Milwaukee Municipal boundaries (Layer -> Add Layer -> Add Vector Layer).  
  
#### Downloading Continent and Boundary Data  
  

