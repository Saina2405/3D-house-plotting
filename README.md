## 3D View of the House Project

This project will create the 3D view of the building present in Flanders region of Belgium with the help of building address.


### Mission Objectives
- Consolidate the knowledge in Python specifically in `Numpy, Pandas` and `Matplotlib`

### Learning Objectives
- Learn how to search and implement new libraries
- Learn how to read and use shapefiles
- Learn how to read and use geoTIFFs
- Learn how to render a 3D plot
- Learn how to present a final product


______________________________________________________________________________________________________________________________________________________

## About The Repository

This is a project about searching an address in Flanders and then it will return a 3D representation of the address using the `LIDAR` method.

`Digital Surface Map (DSM)` and `Digital Terrain Map (DTM)` are already computed and available from www.geopunt.be. We just incorporated it to code to be able to plot the certain address that you wanted to plot. 


### Definition


**LIDAR** is a method to measure distance using light. The device will illuminate a target with a laser light and a sensor will measure the reflection. Differences in wavelenght and return times will be used to get the 3D representations of an area. 

**Digital Surface Model (DSM)** includes ground surface, vegetation and man-made objects. DSM demonstrate the natural and artificial features on the Earth’s surface. DSM may be useful for RF planning, landscape modelling, city modelling, visualization applications and more.

**Digital Terrain Model (DTM)** is often required for flood or ground rupture modeling, land-use studies, geological analysis DSM demonstrate the natural and artificial features on the Earth’s surface.

**Canopy Height Model (CHM)** is the height or residual distance between the ground and the top of the of objects above the ground. This includes the actual heights of trees, builds and any other objects on the earth's surface. The CHM is created by subtracting the DTM from the DSM.


## Repository

This repository has 1 version, namely: 

### Python Notebook version
- If you want to use the notebook version to run the code, all you need is the `3D_houses.ipynb` and the `data` folder to run the code.
- To run the code, you need to input the address that you want and run all the cells to get a 3D representation of the address.

**README.md**
  - has all the necessary information regarding the project

**.gitignore**
  - this contains a list of files that needs to be ignored in the github for example the raster files(DSM and DTM) because they are too big (some are more than 1GB), that way, we wont have any problem uploading the repository to Github

**3D_houses.ipynb**
  - this is the notebook version of the code, if you wish to have only the notebook to run the code it is possible with this code.
  - all you need to do is to use this notebook and the data folder and the code will work and plot the 3D for you

**bounding-box.csv**
  - this is a CSV file containing all the bounding box of the DSM file
  - we will use this csv to figure out which tiff file the address belongs to

**Create_bbox_file.ipynb**
  - Using function to create a list of DSM and DTM raster files and finalized a CSV file


**data folder**
  - this has 4 files namely:
      1. **3D-images folder**
          - this is where all 3D images are saved as a PNG file

      2. **masked-files folder**
          - this is where all the masked files are saved

      3. **temp-raster folder**
          - this is where the tiff files are extracted and saved temporarily, once the program was able to create the masked files, it will then delete the files inside this folder to save storage and memory

      
