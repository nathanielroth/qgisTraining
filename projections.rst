..  _projections:
Projections
===========

Projections take a bit of getting used to in QGIS if you're used to ArcGIS. Most projections are dealt with through specifying their EPSG codes.

QGIS does have a very useful set of tools for searching for and specifying projections.

.. image:: graphics/Projections_01.png

Reproject on the fly is not active by default in QGIS. You need to specify a projection for your project and then turn it on in order to use it. I actually like this feature it is useful for figuring out projections that are either not specified (missing .prj), or incorrectly specified. 

You can access the project's spatial reference settings either through the main menu, or the button at the bottom right of the screen that shows the EPSG code.

.. image:: graphics/Basic_QGIS_12.png

Layers give you a similar dialog for identifying the projection. This can be accessed through the "General" tab on the layer properties. The spatial reference selector remembers your commonly used projections.

.. image:: graphics/Projections_02.png

The website: http://spatialreference.org/ is also very useful.

To reproject vector layers that are in your table of contents, simply right click on the layer name, select "Save As" and in the save as dialog, specify the projection to use through the spatial reference selection dialog.

.. image:: graphics/Projections_02.png

Rasters should be reprojected using the GDAL Warp tools under the *Raster* menu to specify resampling methods and cell sizes. 

