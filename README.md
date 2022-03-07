# 3D Houses Project
![newplot ](https://user-images.githubusercontent.com/96992159/157040491-3516d91c-c4fd-4213-805d-02b0afb3687d.png)



#### Prequisites:
- Python 3.10
- Third Party Files:
  - [DSM](http://www.geopunt.be/download?container=dhm-vlaanderen-ii-dsm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DSM,%20raster,%201m)
  - [DTM](http://www.geopunt.be/download?container=dhm-vlaanderen-ii-dtm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DTM,%20raster,%201m)
- Third Party Libraries:
  - Pandas 0.23.4
  - Numpy Version 1.13.1
  - Matpotlib Version 2.0.2
  - Plotly Version
- API :
  - [Geopunt](https://www.geopunt.be/~/media/geopunt/over%20geopunt/documenten/geopunt%20api.pdf)
  
 #### Objective:
   To build a solution with our `LIDAR Data` to model a house in 3D with only a home address.
   
## Home Address
Any address provided by the user is assessed by `Geopunt API` to get the information about the property such pincode, country, Lambert Coordinates etc . 

## Working with LIDAR files
Using `Rasterio` library `Geotiff` file is read and visualised. The home address is plotted on `Geotiff` file. If the address is not in the file, check in whch file the address exists.

## 3D House
The plotted address on `Geotiff` is cropped to a window using `rasterio.window.from_bounds` and plotted using `Plotly`. 


