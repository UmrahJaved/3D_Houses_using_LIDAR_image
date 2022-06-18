# 3D Houses Project using LIDAR

![maurice](https://user-images.githubusercontent.com/96992159/174431867-0cf3042b-66fd-4540-9819-3f60e3b61572.gif)




* [ Project PPT](https://docs.google.com/presentation/d/1_iGox8LxbZbq-qchUwSBZtLQAxK3sfuWguTtOa1ffR4/edit#slide=id.p)
### Technical Details:

- Data Source:
  - [DSM](http://www.geopunt.be/download?container=dhm-vlaanderen-ii-dsm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DSM,%20raster,%201m)
  - [DTM](http://www.geopunt.be/download?container=dhm-vlaanderen-ii-dtm-raster-1m&title=Digitaal%20Hoogtemodel%20Vlaanderen%20II,%20DTM,%20raster,%201m)
  
- Language:
  - Python 3.10
  
- Used third party libraries:
  - Pandas 0.23.4
  - Numpy Version 1.13.1
  - Matpotlib Version 2.0.2
  - Plotly Version
- Used external API :
  - [Geopunt](https://www.geopunt.be/~/media/geopunt/over%20geopunt/documenten/geopunt%20api.pdf)
  
 #### Objective:
   To build a solution with our `LIDAR Data` to model a house in 3D with only a home address.
   
## Home Address
Any address provided by the user is assessed by `Geopunt API` to get the information about the property such pincode, country, Lambert Coordinates etc . 

## Working with LIDAR files
Using `Rasterio` library `Geotiff` file is read and visualised. The home address is plotted on `Geotiff` file. If the address is not in the file, check in whch file the address exists.

## 3D House
The plotted address on `Geotiff` is cropped to a window using `rasterio.window.from_bounds` and plotted using `Plotly`. 






