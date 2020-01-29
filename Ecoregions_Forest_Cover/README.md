# Automating GIS processes 2019 Final Assignment 

## Topic: 

# Forest area left in naturally forested ecoregions of Europe

Naturally Europe would be largely covered by forests, but human influence has led to deforestation in many areas. My aim is to study the magnitude of this loss from conservation perspective, by comparing amount of forest area left between ecoregions. 

Ecoregions are sub-categories of world biomes defined by WWF, all of them having their own distinct ecological features. In Europe there are about 50 ecoregions, of which about 40 are named as different kinds of forests. Categories refer to potential vegetation, and nowadays in many forest ecoregions the actual forest cover is small. This will be visualized in following  maps and graphs. Results could be used to identify forest types and distinctive natural environments that are the most threatened.

### Notebooks:

- FinalForest1_preparations
- FinalForest2_analysis

### Input data:

- Europe Forest Area raster (100m)
- World Terrestrial Ecoregions 
- World countries

**Europe forest area 2015**

- 100m spatial resolution
- Boolean product of whether the cell is forest or non-forest. Uses FAO definition of forest: minimum coverage of 10% and excluding land that is predominantly under agricultural or urban land use. More info:  
https://sdi.eea.europa.eu/catalogue/srv/eng/catalog.search#/metadata/afe358ed-2c31-4176-8a83-13a530c57091

- **Download link**. In this assignment downloaded to folder "data/forest":  
https://www.eea.europa.eu/data-and-maps/data/european-forest-areas-based-on/european-forest-areas-based-on/forest-area-2015/at_download/file 

Necessary folderpaths are created in the beginning of "FinalForest1_preparations" notebook.

 ![Forestraster](https://autogis-2019.github.io/exercise-5-tyttijussila/forestraster.png)


**Ecoregions shapefile**

- Distinct ecological areas (about 800) defined by WWF. Sub-categories of world biomes. Webmap: 
https://ecoregions2017.appspot.com/

- **Download link** (surprisingly heavy file). In assignment downloaded to folder data/ecoregions:   
http://maps.tnc.org/files/shp/terr-ecoregions-TNC.zip   (Must be unzipped)  
 
 ![Ecoregions](https://autogis-2019.github.io/exercise-5-tyttijussila/ecoregions_vis.png)
 

**World countries shapefile**

- In folder. For masking ecoregions with European countries. 
- Origin:  https://www.naturalearthdata.com/downloads/10m-cultural-vectors/10m-admin-0-countries/

_____________________________________________________________________________________________________________________________  


_____________________________________________________________________________________________________________________________

### Analysis steps:


![Flowchart](https://autogis-2019.github.io/exercise-5-tyttijussila/Final_flowchart.png)


_____________________________________________________________________________________________________________________________  


_____________________________________________________________________________________________________________________________  



### Results:

 ![Graph1](https://autogis-2019.github.io/exercise-5-tyttijussila/forestgraph_percentage.PNG)
 ![Graph2](https://autogis-2019.github.io/exercise-5-tyttijussila/forestgraph_absolute.PNG)
  
 ![Map1](https://autogis-2019.github.io/exercise-5-tyttijussila/forestmap_percentage.png)
 ![Map2](https://autogis-2019.github.io/exercise-5-tyttijussila/forestmap_absolute.png)  
 
 
There are pretty clear patterns. Coastal broadleaf ecoregions have very little forest left, many of them under 10%. This despite the fact that potential dominant vegetation type in these areas is forest. These regions are valuable to human actions and the forests are cut from the way of other land-use. Areas that are more remote, are hard to use for agriculturre, or otherwise have poorer resources or climate, have more forest cover. Of top ten most forested ecoregions nine are mountaineous regions.  


Percentages are interesting, but from conservation and diversity perspective absolute amounts are propably more important. And it seems that these two are not the same - for example Central European Mixed Forests cover quite poor percentage of that ecoregion, but because of its total size the area belongs to Top 5 of Europe in terms of forest area absolute amount.
