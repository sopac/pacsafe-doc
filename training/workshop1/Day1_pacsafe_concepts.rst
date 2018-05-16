.. image:: /images/pacsafe.png

.. _workshop1:

|project_name| concepts
=======================

In this section we explain the key concepts of |project_name| and
explore the merits of disaster management planning.

How does |project_name| work?
-----------------------------

|project_name| combines one exposure layer (e.g. location of
buildings) with one hazard scenario (e.g. the footprint of a tropical
cyclone) and returns a spatial impact layer along with a statistical
summary and action questions. |project_name| is framed around
answering questions such as: "*In the event of a flood similar to the 2012 Nadi event, how many people might need evacuation?*"

.. figure:: /images/001_inasafe_concept.png
   :align: center

   |project_name| concepts.


Definitions
-----------

Before we start, here are some definitions you may find useful. *Other definitions required?*

+---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Risk assessment:**      | *"A methodology to determine the nature and extent of risk by analysing potential hazards and evaluating existing conditions of vulnerability that together could potentially harm exposed people, property, services, livelihoods and the environment on which they depend. "* |
|                           |                                                                                                                                                                                                                                                                                 |
+---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Contingency planning:** | *"A management process that analyses specific potential events or emerging situations that might threaten society or the environment and establishes arrangements in advance to enable timely, effective and appropriate responses to such events and situations."*             |
|                           |                                                                                                                                                                                                                                                                                 |
+---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Response:**             | *"The provision of emergency services and public assistance during or immediately after a disaster in order to save lives, reduce health impacts, ensure public safety and meet the basic subsistence needs of the people affected."*                                           |
|                           |                                                                                                                                                                                                                                                                                 |
+---------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+



Source: 
`http://www.unisdr.org/we/inform/terminology <http://www.unisdr.org/we/inform/terminology>`_

A more complete list of terms is included in the glossary (*link required*).


What is disaster management?
----------------------------

In the context of disaster management, the expected 'normal' situation
is that there is no disaster in progress and people are going about
their normal daily lives. Disaster managers need to plan for the
occasions when the 'normal' situation has been replaced by a disaster
and people can no longer go about their normal daily lives. In order
to prepare for such situations, disaster managers need to have a basic
understanding of questions like:

*   how many people might be in the affected area?
*   how might those people be impacted?



For example are they likely to be injured, stranded, deceased, or
unable to continue with their normal economic activities; have they
lost access to food and water?

*   how will roads in the affected area be impacted?
*   how many dwellings in the affected will be affected? And to what degree?



For example in a flood are buildings dry, wet (but still possibly
habitable) or flooded (with occupants evacuated)?

*   if people are affected, how many of them are likely to be women, children, pregnant, elderly etc.?



Knowing the likely answers to these questions can be helpful to
disaster managers. For example if you are aware of how many people
live in flood prone areas you can estimate how many temporary shelters
might be needed in the event of a disaster, how many provisions should
be stockpiled in order to provide for the daily needs of affected
people and so on. Having demographic breakdowns for the people likely
to be affected, can help disaster managers include things like special
dietary requirements for lactating women in their disaster management
planning.

This planning might also take into account expected impacts on
infrastructure - for example by planning to have sufficient rescue
boats should all the local roads be flooded.

What is a hazard?
-----------------


.. image:: /images/001_inasafe_hazard.png

In the context of |project_name|, a hazard is any natural or human
caused event or series of events that may negatively impact the
population, infrastructure or resources in an area.


Some examples of natural hazards:

*   a flood (caused by overflowing rivers, storm surge, localised precipitation that cannot drain effectively, or by engineering failure such as a dam or levee breach)
*   an earthquake and the resulting ground shaking that is produced by it
*   a tropical cyclone that causes high winds
*   a tsunami



Some examples of non-natural hazards:

*   a chemical spill
*   a power plant failure
*   an industrial fire / explosion



It is important to note that |project_name| is not a hazard modelling
tool. The hazard layers packaged with |project_name| are created
elsewhere. In this training course we will focus on natural hazards,
so we will take a moment here to explain how hazard datasets can be
made.

There are two main ways that can be used to generate hazard datasets:

*   local knowledge; and
*   modelling; 


Local knowledge
...............

This is probably the most practical way to gather hazard data
quickly. One approach that has been effective in Indonesia is to hold
mapping workshops where village chiefs and local officials are
invited. The officials are asked to indicate which villages and
sub-villages within their area of responsibility flood regularly.

Instead of simply mapping which areas are flooded, it is also possible
to take another approach and map each flood event, using the same
boundaries (village). During the event community officials can use
online systems to update the status of the flood waters in their area.

A key requirement for any local knowledge based process is that there
are suitable mapping units available to use for deciding if an area is
flood prone or not. In some cases participants may need to capture
these, in other cases village or sub-village boundaries can be
used. Using administrative boundaries may not always be ideal since
the flood extents are unlikely to align well with the boundaries, but
it may be sufficient for broad planning purposes; especially when
response activities are managed at the same administrative level.

Modelling
.........

Modelling natural hazards is an entire discipline in its own right,
and each of the hazards have vast research communities dedicated to
modelling natural hazards.

Hazard modelling aims to use computer modelss to estimate the magnitude of
hazard phenomena, using empirical, statistical or numerical
representations of the physical characteristics of the hazard
event. For example, to model a flood, we would combine factors such as
precipitation, geology and runoff characteristics, terrain etc. to
derive a model of impending or current flood.

Modelling can use data interpolation techniques - e.g. by taking flood
depth readings manually or using telemetry from various sites around
the flood prone area, flood depths can be interpolated to estimate the
depth at places that were not sampled.

One advantage of using a modelling approach is that it allows us to
forecast less frequent events. For example, there may not be local
knowledge about 1 in 50 or 100 year flood events and their impacts,
but these can be estimated using modelling techniques. A community may
not have experienced a category 5 cyclone, but it may be possible
based on conisderation of the climatic setting. Again, modelling
techniques can enable us to determine what such a cyclone might look
like, and what the likelihood of such a cyclone mught be.

.. _single_vs_multiple:

Single-event versus multiple-event hazards
------------------------------------------

Hazard data used in |project_name| can represent either a single event
or multiple events. Single event hazards are useful when you want to
estimate scenarios like 'how many people would be affected if we had
another flood like in 2013'. A single event hazard covers a short span
of time - like a single flood or earthquake event. Single event data
is also the most suitable to use for events which are stochastic
e.g. earthquakes which seldom occur at the same place and with the
same intensity more than once.

Multiple-event data are useful when you would like to plan for
disasters that repeatedly affect the same area. For example over the
course of 10 years, the same districts or sub-districts may get
flooded, though not on every event. Flood and volcano eruptions may be
good candidates for using multiple-event data in your disaster
management planning.

A more complete description of the available hazard types can be found
in the :ref:`functionality` section of the |project_name| User Guide.



Hazards in InaSAFE
------------------

“In the context of InaSAFE a hazard is any natural or human caused event or series of
events that may negatively impact the population, infrastructure or resources in an
area.”

.. image:: /images/InaSAFE_Exercise_logo.png
You try InaSAFE
---------------
In this exercise we will add in some hazard layers to get a feel of what they represent.

1. Open QGIS
2. Add in the below cyclone hazard datasets using the **add raster layer** button.

*   geonode_fij_w500_tr_west.tif
*   geonode_fij_w500_tr_east.tif

The Cyclone layers will now be displayed in the main window.

.. image:: /images/cyclone_hazard.png

3. Inspect the value of the raster dataset.

What do the values represent?

2. Add in the earthquake hazard dataset (geonode_fij_00_100t.tif) using the **add raster layer** button.

The earth quake layer will now be displayed in the main window.

.. image:: /images/earthquake_hazard.png

3. Inspect the value of the raster dataset.

What do the values represent?

4. Add in the Tsnunami hazard dataset (?.shp) using the **add vector layer** button.

5. Inspect the vector dataset.

What are the hazard classification levels of the Tsunami? (Hint: look in datasets attribute table).



.. image:: /images/questionnaire_logo.png
You try questionnaire
---------------------
Goal: To be able to identify suitable data for use in InaSAFE.

Scenario:
*You are working in a disaster agency and
receive a dataset. Evaluate the dataset in
terms of its suitability for use in InaSAFE. Use
the letter prefixes from the table above to
indicate what the mode, category and
geometry is for each dataset. Put a question
mark if there is no match, and “yes” or “no” to
indicate it the data is suitable. The first item is
completed for you as an example.*

+-----------------------------------------------------------------------------------------------+------------------------+
| Data                                                                                          | Suitable               |
+===============================================================================================+========================+
| A MODIS raster dataset with multiple bands showing flooded areas for a recent flood event.    |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| A shapefile containing flooded areas from a flood last month with a flood depth for each area.|Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| A shapefile containing flood prone areas produced from combining the last 10 flood events.    |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| A single band raster where each cell depicts a flood hazard category of high, medium or low.  |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| A point vector layer showing places where volcano eruptions have taken place.                 |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+

.. image:: /images/tick.png
Check your results:
...................
Swap you list with the person next to you and
see if they had any different ideas about which
consitute valid hazard data.



What is exposure data?
----------------------

In the context of |project_name|, exposure refers to people,
infrastructure or land areas that may be affected by a
disaster. Currently |project_name| supports four kinds of exposure
data:

*   roads
*   buildings
*   population / people
*   landcover


.. _roads:

Roads data
..........


Road datasets are a useful data source when you want to understand the
impact of a flood on roads infrastructure. With the |project_name|
flood on roads impact functions; you can calculate which roads of
which type might be impacted by a flood.

Very often there will be national datasets available for roads. In
this case you should contact your national mapping agency for
up-to-date datasets.  

The OpenStreetMap project is an excellent source of exposure data. The
data is freely available, generally well maintained and a vital
resource for disaster management planners.


There are numerous ways to download OpenStreetMap roads data, but our
recommended way is to download the data using the OSM download tool
provided with |project_name|.

+------------+---------------------------------------------------------------------+
| ** **      | **Key notes for road data**                                         |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Format** | Vector line data                                                    |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Field**  | A field representing road type                                      |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Notes**  | Topologically correct data are best but not essential               |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Source** | Can be obtained from community mapping or a national mapping agency |
|            |                                                                     |
+------------+---------------------------------------------------------------------+


.. _buildings:

Buildings (structure) data
..........................

Like roads, building footprints can be a useful dataset to have for
understanding the impacts of a flood. For example you may wish to know
'how many buildings might be flooded, and what types of buildings are
they?'. In |project_name| you do not need to use engineering quality
data. We are more concerned with the numbers and types of structures
affected by a disaster and do not work at engineering tolerances
needed when, for example, planning a new water mains system.

+------------+---------------------------------------------------------------------+
| ** **      | **Key notes for buildings data**                                    |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Format** | Vector polygon data                                                 |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Field**  | A field representing building type                                  |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Notes**  | PacSAFE does not need 'engineering quality' data                    |
|            |                                                                     |
+------------+---------------------------------------------------------------------+
| **Source** | Can be obtained from community mapping or a national mapping agency |
|            |                                                                     |
+------------+---------------------------------------------------------------------+

.. _population:

Population data
...............


Population data can often be obtained from your census bureau or
through various online data sources. One problem with population data
is that it is often quite coarse (represented using a raster with a
large pixel size) and so analysis at large scales (e.g. a small
neighbourhood) using population data may not always be the best
idea. Currently |project_name| only supports raster based census data,
but in the near future we will be releasing a version that supports
assigning population estimates to buildings using census data. One of
the best online resources for population data is ‘WorldPop’ - a
project that aims to provide population data for anywhere in the globe
produced in a standardised and rigorous way.

+------------------+------------------------------------------------------------+
|                  | **Key notes for population data**                          |
|                  |                                                            |
+------------------+------------------------------------------------------------+
| **Format**       | Raster 'cell' data                                         |
|                  |                                                            |
+------------------+------------------------------------------------------------+
| **Requirements** | Currently the data should be in EPSG:4326 CRS              |
|                  |                                                            |
+------------------+------------------------------------------------------------+
| **Notes**        | Make sure you know if your data represent density or count |
|                  |                                                            |
+------------------+------------------------------------------------------------+
| **Source**       | Can be obtained from a national mapping agency             |
|                  |                                                            |
+------------------+------------------------------------------------------------+

.. _landcover:

Landcover data
..............

Landcover data can often be obtained from national mapping agencies or
through various online data sources. Landcover data are useful if you
want to assess the impact of a hazard event such as a volcanic
eruption on crops.

+------------+-------------------------------------------------------+
| ** **      | **Key notes for landcover data**                      |
|            |                                                       |
+------------+-------------------------------------------------------+
| **Format** | Vector polygon data                                   |
|            |                                                       |
+------------+-------------------------------------------------------+
| **Field**  | A field representing landcover type                   |
|            |                                                       |
+------------+-------------------------------------------------------+
| **Notes**  | Topologically correct data are best but not essential |
|            |                                                       |
+------------+-------------------------------------------------------+
| **Source** | National mapping agency                               |
|            |                                                       |
+------------+-------------------------------------------------------+

.. _aggregation:

.. sidebar:: Sidebar Title
    :subtitle: Optional Sidebar Subtitle

    Subsequent indented lines comprise
    the body of the sidebar, and are
    interpreted as body elements.

.. topic:: Your Topic Title

    Subsequent indented lines comprise
    the body of the topic, and are
    interpreted as body elements.


Exposure in InaSAFE
-------------------
“In the context of InaSAFE, exposure refers to people, infrastructure or land areas that
may be affected by a disaster.”

Currently InaSAFE supports these kinds of exposure data: population / people, roads,
buildings, places, landcover. Exposure datasets need to comply with these modes and
geometries:

+--------------------+-----------------------------------------------+
| **Exposure Modes** | **Exposure Geometries**                       |
+--------------------+------------------+----------------------------+
| a) Coninuous data  | c) Vector points | e) Vector polygons         |
+--------------------+------------------+----------------------------+
| b) Classified data | d) Vector lines  | f) Single band rasters     |
+--------------------+------------------+----------------------------+

.. image:: /images/questionnaire_logo.png
You try questionnaire
---------------------
Goal: To be able to identify suitable data for use in InaSAFE.

*Complete the table below by indicating
one example exposure type for each geometry
type and mode. The first entry has been
completed for you as an example.*

+-----------------------------------------------------------------------------------------------+------------------------+
| **Dataset**                                                                                   | **Example**            |
+===============================================================================================+========================+
| Continuous data                                                                               | Population areas       |
+-----------------------------------------------------------------------------------------------+------------------------+
| Classified data                                                                               |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| Vector points                                                                                 |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| Vector lines                                                                                  |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| Vector Polygons                                                                               |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+
| Single band rasters                                                                           |Y/N                     |
+-----------------------------------------------------------------------------------------------+------------------------+

.. image:: /images/tick.png
Check your results:
...................
Swap you list with the person next to you and
see if they had any different ideas about which
consitute valid hazard data.


.. image:: /images/InaSAFE_Exercise_logo.png
You try InaSAFE
---------------
In this exercise we will add in some exposure layers, perform a basic selection query and symbolise buildings on wall type.

1. Open QGIS

2. Add in the buildings exposure dataset using the **add vector layer** button.

The buildings vector layer will now be displayed in the main window.

3. Open the attribute table of the buildings layer by right clicking on the layer name in the layers panel and selecting **Open attribute table**.

Notice the fields and values that the buildings layer contains.

4. In the attribute table, click **Select features using expression** button.

The select by expression window appears with some calculation buttons (Operators) and a textbox at the bottom into
which are typed search expressions (SQL where clause).

5. Create a query to select the buildings with brick wall type.

Notice at the top of the attribute table telling you that number of buildings that have brick wall type.

Now we will symbolise the buildings layer to visually display the different wall types of the buildings.

6. Right click the buildings layer in the table of contents and select **Properties**.

7. In the window that opens select the **Style** tab.

8. At the very top of window select the first drop down list and select **Categorised** from the drop down list.

9. Under the **Column** drop down list, select the name of the attribute field you want to symbolize on your map, which in this case is **Wall_type**.

This will display a list of classes, one for each unique value from the **Wall_type** class
is assigned a colour symbol. Unless specific colours are selected, QGIS will assign random
colours, one for each class.

10. Select **OK** and view the results.

What is aggregation?
--------------------

Aggregation is the process whereby we group the results of the
analysis by district so that you can see how many people, roads or
buildings were affected in each area. This will help you to understand
where the most critical needs are, and to generate reports as shown in
the image below. Aggregation is optional in |project_name| - if you do
not use aggregation, the entire analysis area will be used for the
data summaries. Typically aggregation layers in |project_name| have as
attributes the name of the district, village or reporting area. It is
also possible to use extended attributes to indicate the ratio of men
and women; youth, adults and elderly living in each area. Where these
are provided and the exposure layer is population, |project_name| will
provide a demographic breakdown per aggregation area indicating how
many men, women etc. were probably affected in that area.

While it is not required to use aggregation areas in InaSAFE, it is recommended.
Aggregation areas are typically political boundaries: wards, villages, districts, provinces
etc. Generally disasters are more localised in scale, so using smaller aggregation units
often makes sense. Currently InaSAFE supports only vector polygon datasets for use as
aggregation layers. The aggregation layer used will also determine the analysis area
when running an analysis in InaSAFE. If a QGIS selection has been made on an
aggregation layer, the analysis will be constrained to only the selected areas.


.. figure:: /images/001_tonga_villages.png

   Example of aggregation data for Tongatapu. In this case the aggregation
   areas are villages. Source: PCRAFI.


.. image:: /images/questionnaire_logo.png
You try questionnaire
---------------------
Goal: To be able to understand the importance of aggregation data in InaSAFE.

*Think about a disaster prone area in your
community. Now think about contingency
planning and post disaster support operations
for that area. What aggregation area unit
(ward, village, district, etc.) makes the most
sense, and why? Use the space provided in the table below
for your answer and jot down a few
keywords justifying your choice.*

+-----------------------------------------------------------------------------------------------+------------------------+
| **Aggregation Unit**                                                                          |                        |
+===============================================================================================+========================+
| Reasoning                                                                                     |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
|                                                                                               |                        |
+-----------------------------------------------------------------------------------------------+------------------------+

.. image:: /images/tick.png
Check your results:
...................
Swap you list with the person next to you and
see if they had any different ideas about which
consitute valid hazard data.


.. image:: /images/InaSAFE_Exercise_logo.png
You try InaSAFE
---------------
In this exercise you will add in layers that can be used to aggregate inasafe results within specific administation
boundaries.

1. Add in the below Fiji village and division boundary datasets using the **add vector layer** button.

*   fji_polbnda_adm0_country.shp
*   fji_polbnda_adm1_district.shp
*   fji_polbnda_adm2_province.shp
*   fji_polbnda_adm3_tikina.shp

These administration layers will now be displayed in the main window.

2. Inspect each layer, noticing the differences in each.

These layers can each be used to group or aggregate the results of the analysis.


What is contextual data?
------------------------

Contextual data are data that provide a sense of place and scale when
preparing or viewing the results of analysis, while not actually being
used for the analysis. For example you may include online maps to show
the underlying relief of the study area, or an aerial image to show
what buildings and infrastructure exist in the area.

.. figure:: /images/001_tonga_aerial.png
   
    Aerial imagery for Nuku'alofa, Tonga. Source: PCRAFI.

A practical example using InaSAFE with OSM data
...............................................
We mentioned in the overview of exposure data that these data can be easily obtained
from OpenStreetmap in InaSAFE. In fact InaSAFE have built a service that extracts exposure
data from OSM, cleans the data, applies standard symbology to it, adds InaSAFE
keywords, packs everything up in a zip file for easy use in InaSAFE. The service runs on
an internet server (http://osm.inasafe.org) so requires internet connectivity to use. We
have built a client for the service directly into InaSAFE.

.. image:: /images/InaSAFE_Exercise_logo.png
You try InaSAFE
---------------
Goal: To be able to add data from OSM.

1. In QGIS look in your InaSAFE toolbar for the OpenStreetmap Downloader.

.. image:: /images/InaSAFE_toolbar_OSM.png


2. Run the downloader with the following options.

.. image:: /images/OSM_downloader.png


3. Click on the **Drag on map** button and select an area where you want to download the OSM data.

After the data has downloaded, you will notice the data will appear in QGIS.

Is the data you downloaded hazard data, exposure data or aggregate data?

4. ...create steps for imagery plugins using web services...

What is the difference between raster and vector data?
------------------------------------------------------

Vector data is arguably the most common kind of data you will find in
the daily use of GIS. It describes geographic data in terms of points
that may be connected into lines and polygons. Every object in a
vector dataset is called a feature, and is associated with data that
describes that feature. The basic shape of objects stored in the
vector data is defined with a two-dimensional coordinate system /
Cartesian (x, y).

.. figure:: /images/001_vector_data.png
   :align: center 

   Examples of vector data.


Raster data is different from vector data. While vector data has
discrete features constructed out of vertices, and perhaps connected
with lines and/or areas; raster data, is like an image. Although it
may portray various properties of objects in the real world, these
objects don't exist as separate objects; rather, they are represented
using pixels or cells of various different numerical values. These
values can be real and represent different characteristics of the
geography, such as water depth or amount of volcanic ash; or they can
be a code than is related to the type of land use or the hazard class.

.. figure:: /images/001_raster_data.png
   :align: center 

   Example of raster data.

.. note:: Creating vector data is like using a pen, where you can draw
          a point, a line or a polygon, Raster data is like taking a
          picture with a camera, where each square has one value, and
          all the squares (pixels) combine to make a picture.

Both vector and raster data can be used in |project_name|. For
example, we use vector data for the extent of a flood hazard and as
well as roads and building footprint; but we use raster data for
modelled hazards such as flood depth, tsunami inundation and for
population exposure.

.. _continuous_vs_classified:



What is the difference between continuous and classified data?
--------------------------------------------------------------

In |project_name| we differentiate between data which is continuous
and data which is classified. The terms can be applied equally to both
hazard and exposure data.


**Continuous** data represent a **continuously varying phenomenon**
 such as depth in meters, population counts and so on.

.. figure:: /images/001_continuous_data.png

   Example of continuous population data, displayed in GIS software. Source WorldPop.

**Classified data** represent **named groups of values**, for example,
high, medium and low hazard. Grouping values works well when you wish
to reduce data preparation complexity or deal with local variances in
the interpretation of data. For example, a flood depth of 50Â cm may
represent a high hazard zone in an area where people commonly have
basements in their houses, and a low hazard zone in areas where
people commonly build their houses on raised platforms.

.. figure:: /images/001_classified_data.png

   Classified raster flood data - courtesy BNPB/Australian Government


What is an Impact Function?
---------------------------

.. image:: /images/001_impact_function.png
   :align: center
   :width: 300 pt

An Impact Function (often abbreviated to IF) is software code in
|project_name| that implements a particular algorithm to determine the
impact of a hazard on the selected exposure. Running an impact
function is done when you have prepared all your input data, defined
your analysis extent and wish to now see the impact outputs.

Again, we should emphasise here that Impact Functions **do not model hazards**
- they **model the effects** of one or more hazard events on an
exposure layer.  |project_name| groups its impact functions according
to the kind of hazard they work on:

The Impact Function Wizard will guide you through the process of
setting up a |project_name| assessment. The starting point of the
Wizard displays the available combinations of hazard and exposure
layers for which there are Impact Functions.

.. figure:: /images/impact_wizard.png
   :align: center

   |project_name| Impact Function Wizard demonstrating possible
   exposure and hazard combinations.


.. image:: /images/InaSAFE_Exercise_logo.png


You try InaSAFE
---------------

Goal: View the **Impact function** and get an understanding of the steps in running a guided impact assessment.

1. In QGIS add in the following hazard and exposure datasets

+-----------------------------------------------------------------------------------------------+------------------------+
| **Hazards**                                                                                   | **Exposures**          |
+===============================================================================================+========================+
| Tsunami flood extent                                                                          | Population             |
+-----------------------------------------------------------------------------------------------+------------------------+
| Cyclone wind                                                                                  | Buildings              |
+-----------------------------------------------------------------------------------------------+------------------------+

2. Click on the **Impact function**

.. image:: /images/InaSAFE_toolbar_Impact_function.png





Supported data types for each hazard type in |project_name|
-----------------------------------------------------------
.. image:: /images/icon_earthquake.png
   :align: left

Earthquake Impact Functions
...........................

**Earthquake hazard**:  continuous raster, classified raster, and classified polygon

**Population exposure**: continuous raster with counts

**Building exposure**: classified polygon or point with a type attribute



.. image:: /images/icon_flood.png
   :align: left

Flood Impact Functions
......................

**Flood hazard**:  continuous raster or classified polygon

**Population exposure**: continuous raster with counts

**Building exposure**: classified polygon or point with a type attribute

**Road exposure**: classified line with a type attribute



.. image:: /images/icon_tsunami.png
   :align: left

Tsunami Impact Functions
........................

**Tsunami hazard**: continuous raster or classified polygon

**Population exposure**: continuous raster with counts

**Building exposure**: classified polygon with a type attribute

**Road exposure**: classified line with a type attribute



.. image:: /images/icon_volcano.png
   :align: left

Volcano Impact Functions
........................

**Volcano hazard**:  continuous polygon, classified polygon, and point

**Population exposure**: continuous raster with counts

**Building exposure**: classified polygon with a type attribute



.. image:: /images/icon_volcanic_ash.png
   :align: left

Volcanic Ash Impact Functions
.............................

**Volcano hazard**:  clasified polygon or continuous raster

**Population exposure**: continuous raster with counts

**Building exposure**: classified polygon with a type attribute


.. image:: /images/icon_cyclone.png
   :align: left

Cyclone Impact Functions
........................

**Cyclone hazard**: continuous raster

**Building exposure**: classified polygon or point with a type attribute.


.. image:: /images/icon_generic.png
   :align: left

Generic Impact Functions
........................

**Volcano hazard**:  classified polygon, classified raster or continuous raster

**Population exposure**: continuous raster with counts

**Building exposure**: classified polygon with a type attribute

**Landcover exposure**: classified polygon with a type attribute

A note about generic impact functions: Generic IF's are useful when your
data does not conform to the a priori expectations of |project_name|.
For example, you may wish to produce a report on buildings that might be
affected by a landslide, drought, smoke haze or any other hazard that does not
have an explicit Impact Function in |project_name|.

Each Impact Function will generate outputs that may include:
- an impact map layer
- an impact summary
- minimum needs
- action checklists

.. image:: /images/001_inasafe_output.png
   :align: center
   :width: 300 pt

Summary
-------

In this session, we explored the concepts underpinning |project_name|,
covering disaster management, what are the elements that contribute to
impact assessment, and introduced common terms you will hear
throughout the rest of the training workshop that are specific to the
|project_name| application.
