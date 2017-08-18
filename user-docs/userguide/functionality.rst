.. _userguide:

Data Requirements
=================

This document describes the data requirements of |project_name| in regard to what
inputs are needed to carry out an analysis.

At the highest level |project_name| will take a hazard layer (such as ground
shaking, water depth or ash load) and an exposure layer (such as population
density or building footprints) and combine them according to an impact
function to produce an impact layer and a report.

Hazard layers
-------------

The supported hazard layers are:

+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Hazard     |Spatial type |Hazard type        |Attribute name |Hazard units/fields |Parameters    |
+===========+=============+===================+===============+====================+==============+
|Volcano    |Raster       |Ash load           |N/A            |kg/m^2              |              |
+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Volcano    |Point        |Distance from vent |Name           |text                |Radius [km]   |
+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Volcano    |Polygon      |Category           |KRB            |text                |              |
+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Earthquake |Raster       |Shakemap           |N/A            |MMI                 |              |
+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Flood      |Raster       |Depth              |N/A            |m                   |Threshold [m] |
+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Flood      |Polygon      |Wet/Dry            |affected       |1/0                 |Threshold [%] |
+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Tsunami    |Raster       |Depth              |N/A            |m                   |Threshold [m] |
+-----------+-------------+-------------------+---------------+--------------------+--------------+
|Cyclone    |Raster       |Wind speed         |N/A            |m/s                 |Category      |
+-----------+-------------+-------------------+---------------+--------------------+--------------+

Exposure layers
---------------

==========  ============ ==================  ============== ===================
Exposure    Spatial type Exposure type       Attribute name Hazard units/fields
==========  ============ ==================  ============== ===================
Population  Raster       Density             N/A            People per pixel
Structures  Point        Structure type      type           text
Structures  Polygon      Structure type      type           text
Roads       Polyline     Road type           type           text
Land cover  Polygon      Land cover type     type           text
==========  ============ ==================  ============== ===================
