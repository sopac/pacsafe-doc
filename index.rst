PacSAFE Training Workshop - Tonga
=================================

*Tonga, April, 2017*

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   objectives
   introduction
   concepts

.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`







What is an Impact Function?
===========================

|10000201000004270000021EB2807F8F2C80E98E_png|

An Impact Function (often abbreviated to IF) is software code in PacSAFE that implements a particular algorithm to determine the impact of a hazard on the selected exposure. Running an impact function is done when you have prepared all your input data, defined your analysis extent and wish to now see the impact outputs.

Again, we should emphasise here that Impact Functions do not model hazards - they model the effects of one or more hazard events on an exposure layer. PacSAFE groups its impact functions according to the kind of hazard they work on:

*Supported data types for each hazard type in InaSAFE:*

|100002010000004400000044CC8C90B40B155577_png|
**Earthquake Impact Functions**

Earthquake hazard: continuous raster, classified raster, and classified polygon

Population exposure: continuous raster with counts

Building exposure: classified polygon or point with a type attribute


|100002010000004400000043EAFCCD2DA5D63DDE_png|
**Flood Impact Functions**

Flood hazard: continuous raster or classified polygon

Population exposure: continuous raster with counts

Building exposure: classified polygon or point with a type attribute

Road exposure: classified line with a type attribute

|1000020100000043000000442857E450D7916541_png|
**Tsunami Impact Functions**

Tsunami hazard: continuous raster or classified polygon

Population exposure: continuous raster with counts

Building exposure: classified polygon with a type attribute

Road exposure: classified line with a type attribute


|1000020100000044000000445540F66CD7333DAE_png|
**Volcano Impact Functions**

Volcano hazard: continuous polygon, classified polygon, and point

Population exposure: continuous raster with counts

Building exposure: classified polygon with a type attribute


|1000020100000044000000443D54B4E784144E4C_png|
**Volcanic Ash Impact Functions**

Volcano hazard: classified polygon or continuous raster

Population exposure: continuous raster with counts

Building exposure: classified polygon with a type attribute

|100002010000009C0000009C43C8B8C251794B3E_png|
**Cyclone Impact Functions**

Cyclone hazard: continuous or classified polygon, continuous or classified raster

Population exposure: continuous raster with counts

Building exposure: classified polygon with a type attribute


|10000201000000440000004452F6510DADA0A162_png|
**Generic Impact Functions**

Volcano hazard: classified polygon, classified raster or continuous raster

Population exposure: continuous raster with counts

Building exposure: classified polygon with a type attribute

Landcover exposure: classified polygon with a type attribute

A note about generic impact functions: Generic IF’s are useful when your data does not conform to the a priori expectations of PacSAFE. For example, you may wish to produce a report on buildings that might be affected by a landslide, drought, smoke haze or any other hazard that does not have an explicit Impact Function in PacSAFE.


Each Impact Function will generate outputs that may include: - an impact map layer - an impact summary - minimum needs - action checklists


|10000201000005860000018B95ECE8E7C303FD6B_png|
**What is an impact layer?**

An impact layer is a new GIS dataset that is produced as the result of running an impact function. It will usually represent the exposure layer. For example, if you do a flood analysis on buildings, the impact layer produced will be a buildings layer but each building will be classified according to whether it is dry, wet or flooded. PacSAFE will typically apply its own symbology to the output impact layer to make it clear which are the impacted buildings. This is illustrated in the image below.

It should also be noted that the impact layer will only include features / cells that occur within the analysis extent. All others will be ‘clipped away’. It is very important to remember this when interpreting the map legend and the impact summary (see section below) because they are only relevant to the analysis area. The impact layer is not saved by default. If you want to save this spatial data you need to do this yourself.


|1000020100000498000004CC90E5D7823F02EB7A_png|

**What is the impact summary?**

Whereas the impact layer represents spatial data, the impact summary is tabular and textual data. The impact summary provides a table (or series of tables) and other textual information with the numbers of buildings, roads or people affected, and includes other useful information such as minimum needs breakdowns, action checklists and summaries. The impact summary presents the results of the impact function in an easy to digest form. Our expectation that the numbers show here would form part of the input to your emergency management planning process - typically as a launch point for discussion and planning on how to have sufficient resources in order to cater for the impacted people, buildings or roads should a similar event to the one on which the scenario is based occur. An example of an impact summary is shown below.


|1000020100000568000003854B3E041BB1044C14_png|

*Figure *
*: Example impact summary table showing breakdown of buildings flooded.*

**What are minimum needs?**

Minimum needs are a population specific reporting component for the impact summary. They are based on generic or regional preferences and define the daily food and well-being requirements for each individual who may be displaced during a disaster. For example you could specify that each person should receive 20l of fresh drinking water per day, 50l of bathing water and so on. PacSAFE will calculate these numbers to provide an estimate of the total needs for the displaced population.


|10000201000003AD000000CEA674FD7370360E6F_png|

**What are action checklists?**

Action checklists are generated lists of things disaster managers should consider when implementing their disaster management plan. Currently the action checklists are fairly simplistic - they are intended to prompt discussion and stimulate disaster managers to think about the important contingencies they should have in place.


|10000201000002E0000001C2CEDFED88A69ED83E_png|

**Datasets**

*Current content has InaSAFE specific datasets – need to update in consultation with Sachin & Lauren*

Introduction to PacSAFE
=======================

Introduction

Learning objectives

*   Understand how to install PacSAFE



*   Introduction to the PacSAFE toolbar and functionality



*   Learn basic operations in PacSAFE



Exercises
=========

**Getting PacSAFE**

**Installing PacSAFE**

**Understanding the PacSAFE interface**

**PacSAFE basic tools**

**Navigating the map**

**Hide and move layers**

**Symbolize a layer**

**PacSAFE toolbar**

**Summary**

Run PacSAFE
===========

**Introduction**

In this exercise, we will work through an example scenario where we show how the different data elements used by PacSAFE are combined in order to analyse the potential impact of a tsunami on both the buildings and population.

After we have run the PacSAFE analysis we will print the map and analysis report as a pdf and review the results. We will also learn how to change the inundation threshold and take a look at the default settings for minimum needs. We will also learn how to save our work.

**Learning objective**

To develop the participant’s basic understanding of the InaSAFE workflow and application of InaSAFE in the Disaster Management sector. By the end of this exercise, participants will:


*   Be able to run a tsunami analysis using PacSAFE - on buildings;



*   Be able to run a tsunami analysis using PacSAFE - on population;



*   Understand the tsunami impact default settings;



*   Understand the impact summary report;



*   Be able to change the analysis threshold and run a new scenario;



*   Be able to generate a PDF map from the results of an analysis; and



*   Be able to save their work to share results with others.



*Data for this exercise*

The data for this exercise are
packaged in the PacSAFE application.
There is no need to download data to run the exercises.

.. |1000000000000148000000763C22F77D7C299FDD_jpg| image:: images/1000000000000148000000763C22F77D7C299FDD.jpg


.. |100002010000057C0000039673F261A1F4F33886_png| image:: images/100002010000057C0000039673F261A1F4F33886.png


.. |10000000000002A20000012DD9625173C0124347_png| image:: images/10000000000002A20000012DD9625173C0124347.png
    :width: 16cm
    :height: 7.146cm


.. |10000000000002AE00000156F2C6DD5A4FA21026_png| image:: images/10000000000002AE00000156F2C6DD5A4FA21026.png
    :width: 16cm
    :height: 7.976cm


.. |10000000000002A7000001268F8C19B2DCDC3F44_png| image:: images/10000000000002A7000001268F8C19B2DCDC3F44.png
    :width: 16cm
    :height: 6.929cm


.. |1000020100000174000001554CDAA6814BF94AB3_png| image:: images/1000020100000174000001554CDAA6814BF94AB3.png


.. |100002010000007D0000005F573048AF9A3DA6CA_png| image:: images/100002010000007D0000005F573048AF9A3DA6CA.png


.. |100000000000039000000317A7A613669932E370_png| image:: images/100000000000039000000317A7A613669932E370.png
    :width: 16cm
    :height: 13.416cm


.. |100000000000039000000317058BA88F87534130_png| image:: images/100000000000039000000317058BA88F87534130.png
    :width: 15.99cm
    :height: 13.416cm


.. |100000000000017B000000F871DFDD7DBF63B3C2_png| image:: images/100000000000017B000000F871DFDD7DBF63B3C2.png


.. |10000000000000AA000000AA2CAF21F3194C7C22_png| image:: images/10000000000000AA000000AA2CAF21F3194C7C22.png


.. |100002010000056A00000313CCF9848F176DC3DC_png| image:: images/100002010000056A00000313CCF9848F176DC3DC.png


.. |100002010000056B0000034B293CE5D07B3DFB82_png| image:: images/100002010000056B0000034B293CE5D07B3DFB82.png


.. |100002010000039F00000355996C0DC117FE9AD6_png| image:: images/100002010000039F00000355996C0DC117FE9AD6.png


.. |10000201000004270000021EB2807F8F2C80E98E_png| image:: images/10000201000004270000021EB2807F8F2C80E98E.png


.. |100002010000004400000044CC8C90B40B155577_png| image:: images/100002010000004400000044CC8C90B40B155577.png


.. |100002010000004400000043EAFCCD2DA5D63DDE_png| image:: images/100002010000004400000043EAFCCD2DA5D63DDE.png


.. |1000020100000043000000442857E450D7916541_png| image:: images/1000020100000043000000442857E450D7916541.png


.. |1000020100000044000000445540F66CD7333DAE_png| image:: images/1000020100000044000000445540F66CD7333DAE.png


.. |1000020100000044000000443D54B4E784144E4C_png| image:: images/1000020100000044000000443D54B4E784144E4C.png


.. |100002010000009C0000009C43C8B8C251794B3E_png| image:: images/100002010000009C0000009C43C8B8C251794B3E.png


.. |10000201000000440000004452F6510DADA0A162_png| image:: images/10000201000000440000004452F6510DADA0A162.png


.. |10000201000005860000018B95ECE8E7C303FD6B_png| image:: images/10000201000005860000018B95ECE8E7C303FD6B.png


.. |1000020100000498000004CC90E5D7823F02EB7A_png| image:: images/1000020100000498000004CC90E5D7823F02EB7A.png


.. |1000020100000568000003854B3E041BB1044C14_png| image:: images/1000020100000568000003854B3E041BB1044C14.png


.. |10000201000003AD000000CEA674FD7370360E6F_png| image:: images/10000201000003AD000000CEA674FD7370360E6F.png


.. |10000201000002E0000001C2CEDFED88A69ED83E_png| image:: images/10000201000002E0000001C2CEDFED88A69ED83E.png

