.. image:: /images/pacsafe.png

.. _workshop1:

Run basic |project_name|
========================

Introduction
------------

In this module, we will learn about the results of a InaSAFE analysis and work through an example scenario where we
show how the different data elements used by |project_name| are combined in order to analyse the potential impact of a
tsunami on both the buildings and population.

After we have run the |project_name| analysis we will print the map and
analysis report as a pdf and review the results. We will also learn
how to change the inundation threshold and take a look at the default
settings for minimum needs. We will also learn how to save our work.

Learning objective
..................

To develop the participant's basic understanding of the |project_name|
workflow and application of |project_name| in the Disaster Management
sector. By the end of this exercise, participants will:


*   Be able to run a tsunami analysis using |project_name| - on buildings;
*   Be able to run a tsunami analysis using |project_name| - on population;
*   Understand the tsunami impact default settings;
*   Understand the impact summary report;
*   Be able to change the analysis threshold and run a new scenario;
*   Be able to generate a PDF map from the results of an analysis; and
*   Be able to save their work to share results with others.


What is an impact layer?
------------------------
An impact layer is a new GIS dataset that is produced as the result of
running an impact function. It will usually represent the exposure layer.
For example, if you do a flood  analysis on buildings, the impact layer
produced will be a buildings layer but each building will be classified
according to whether it is dry, wet or flooded. |project_name| will typically
apply its own symbology to the output impact layer to make it clear which
are the impacted buildings. This is illustrated in the image below.

It should also be noted that the impact layer will only include features /
cells that occur within the analysis extent. All others will be 'clipped away'.
It is very important to remember this when interpreting the map legend and the
impact summary (see section below) because they are only relevant to the
analysis area.  The impact layer is not saved by default. If you want to
save this spatial data you need to do this yourself.

.. image:: /images/001_building_output.png
   :align: center
   :width: 300 pt

What is the impact summary?
---------------------------
Whereas the impact layer represents spatial data, the impact summary is
tabular and textual data. The impact summary provides a table (or series of
tables) and other textual information with the numbers of buildings, roads or
people affected, and includes other useful information such as minimum needs
breakdowns, action checklists and summaries. The impact summary presents the
results of the impact function in an easy to digest form. Our expectation that
the numbers show here would form part of the input to your emergency
management planning process - typically as a launch point for discussion and
planning on how to have sufficient resources in order to cater for the
impacted people, buildings or roads should a similar event to the one on
which the scenario is based occur.

An example of an impact summary is shown below.

.. image:: /images/001_impact_summary_buildings.png
   :align: center
   :width: 600 pt

Example impact summary table showing breakdown of buildings flooded.

What are minimum needs?
-----------------------
Minimum needs are a population specific reporting component for the
impact summary. They are based on generic or regional preferences and define
the daily food and well-being requirements for each individual who may be
displaced during a disaster. For example you could specify that each person
should receive 20l of fresh drinking water per day, 50l of bathing water and
so on. |project_name| will calculate these numbers to provide an estimate of
the total needs for the displaced population.

.. image:: /images/001_impact_summary_min_needs.png
   :align: center
   :width: 600 pt

What are action checklists?
---------------------------
Action checklists are generated lists of things disaster managers should
consider when implementing their disaster management plan. Currently the
action checklists are fairly simplistic - they are intended to prompt
discussion and stimulate disaster managers to think about the important
contingencies they should have in place.

.. image:: /images/001_impact_summary_actions.png
   :align: center
   :width: 300 pt



Data for this exercise
......................

The data for this exercise are packaged in the |project_name|
application. There is no need to download data to run the exercises.

Exercise
--------

Open |project_name| application
...............................

Before running a |project_name| analysis, we must open a
project. Start |project_name| by double clicking the |project_name|
icon on the desktop.

.. image:: /images/icon.png
   :align: center


A splash screen will appear for a few seconds, then the main
|project_name| interface will be displayed.

.. image:: /images/splash.png
   :align: center


Choose a disaster scenario
..........................

Clicking on the |project_name| button in the |project_name| toolbar
will open a new window, with a list of projects that you can select
from.

.. figure:: /images/001_project_selection.png
   :align: center

   Project selection window for |project_name|.

We will start by examining the scenario of a tsunami and it's impact
on buildings in and around Nuku'alofa. Select the "Nukualofa tsunami
buildings" project in the list, then click the :guilabel:`Load` button.

The project will show several layers in the Layers panel, including:

* Buildings: this is the exposure data. This will be used to assess
  the tsunami impact on buildings.
* Tsunami: this is the hazard data. It is used to determine the
  inundation depth from a tsunami.
* Imagery: this is contextual data, and is aerial imagery over
  Nuku'alofa. This provides a sense of place and scale when viewing
  the results of analysis. It is not used in the analysis.

Use the panning tools to navigate around the map
(:ref:`navigate`). You might want to find your home, or a local
school.

.. image:: /images/map_navigation.png
   :align: center


The contextual data should help you to find features of interest, such
as your home, local school, or church.

Run |project_name| analysis for buildings
-----------------------------------------

Take a look at the |project_name| dock on the right side of the
screen. The |project_name| dock should show that you are ready to run
a tsunami analysis. It poses the question "in the event of **a tsunami
generated by a Mw 8.7 earthquake**, how many **buildings** might **be
inundated**?". This analysis will use the default thresholds for low,
medium and high hazard zones - we will explore that later.

.. figure:: /images/001_analysis_setup.png
   :align: center

   |project_name| dock showing it is ready to run an analysis.

Notice that the third element in the |project_name| dock, under
"Summarise the results by" is greyed out. This option is used for
aggregating the results (:ref:`aggregation`). We will cover
aggregation in a later exercise.

Click the :guilabel:`Run` button in the lower right corner of the
|project_name| dock to start the analysis process. After a few
seconds, you should get a result in the dock area, and several new
layers should be added to the map. You will see these new layers
listed at the top of the Layers panel.

.. figure:: /images/001_layers_tsunami_building_results.png
   :align: center

   Layers panel after running the tsunami on buildings analysis.


Interpret the results
.....................

The new impact layer will be generated and called **Estimated buildings
affected**. Let's take a look at the new impact layer
generated by |project_name|.

- Zoom in to some area on the map canvas

- Here, we zoomed in to an area near the centre of Nuku'alofa. There
  will be different colours generated from |project_name| (green,
  yellow, orange, red).

.. image:: /images/001_basic_pacsafe_impact_layer_zoom.png
   :align: center
   :width: 400 pt

.. note:: If you dont see these colours, you might need to turn off
          the data layer above the "Estimated buildings affected"
          layer.

.. note:: In this analysis, there are very few green buildings so
          there may not be any in the map extents.

- The building points are all coloured according to the depth of inundation, or **hazard zone**:

  * The red buildings points are inundated to a depth of 3 metres or more (**High hazard**)
  * Orange building points inundated between 1.0 and 3.0 metres (**Medium hazard**)
  * Yellow building points are inundated between 0.1 and 1.0 metres (**Low hazard**)
  * Green building points are inundated no more than 0.1 metres (**Dry**)
  * Grey building points are considered **unaffected**, as they are
    situated in dry areas according to the inundation model.
  

Click :guilabel:`Number of buildings` in the layer list to select it
and click :guilabel:`Identify Feature` tool and then click on a
building to view the attributes of that building.

.. figure:: /images/001_basic_pacsafe_feature_table.png
   :align: center
   :width: 300 pt



In the |project_name| panel we now see the impact summary. The details
of this summary table are explained below.

.. figure:: /images/001_basic_pacsafe_impact_summary.png
   :align: center
   :width: 250 pt

   PacSAFE Impact summary, as viewed in the PacSAFE dock.

The first section, titled **General report**, contains a count of the
numbers of buildings in each hazard zone, and those considered
affected or unaffected.



-  **Hazard Zone**: divides the results into several categories
   based on the threshold set in the hazard analysis. In this impact
   summary, |project_name| divides the impact buildings into two
   categories: number of buildings in **Medium** or **High** hazard
   zones - labeled *affected* (buildings inundated by more than 1.0
   metres of water) and those considered *not affected*, which are
   those buildings in a **Low** hazard zone or **Dry** (buildings not
   affected by any water).

-  **Structure type:** divides the exposed buildings into several
   categories based on the building type attribute for each
   building. In this impact summary, |project_name| breaks down the results
   into a more detailed report by looking at each type of the
   building, for example the number of inundated hospitals and the
   total number of hospitals in analysis area.

-  **Action checklist:** designed to make disaster managers think about
   what they need to do/discuss when planning for a similar event in
   the future.

-  **Notes and assumptions:** provides details about the input data and
   any limitations or assumptions in the analysis or report
   summary. In this example, it explains why buildings are said to be
   inundated, wet and dry.

-  **Aggregation result:** statistical breakdown of the building
   types affected by the simulated event. When you choose to use an aggregation
   layer with your analysis (we will do this later) this table will show the
   number of buildings by aggregation boundary (such as villages).

-  **Analysis details:** explains where the hazard and exposure data
   come from, the aggregation data and the type of impact function
   used in the analysis. In this case, the **Hazard source** is named
   "Tsunami from Mw 9.0 earthquake - PSLP", the **Exposure source** is
   listed as "PCRAFI", the **Aggregation source** is not used and the
   **Impact Function** is "Tsunami Raster on Structure Point".

The results show the buildings that will be affected by tsunami
inundation of greater than 1.0 metres of water. But what if the
disaster manager decides that buildings in 50cm of water are also
affected? In order to assess this new scenario, we need to change the
water depth threshold at which buildings are considered to be
inundated.

With |project_name| it is easy to run a new scenario, all you need to
do is change the **Thresholds [m]** in the Options tab to 0.5 metres
and run the scenario again.  We will do this in a later session.



Reading the Impact Summary report
.................................

The Impact Summary report contains the details of the impact analysis
in tables for ease of reading.


.. figure:: /images/001_impact_summary_tsunami_buildings.png
   :align: center

   Impact summary report for tsunami on buildings analysis.

Notice how the "Analysis detail" section has sub-headings "High hazard
zone", "Medium hazard zone" and "Low hazard zone"? You can select the
thresholds that define these zones, using the "Keyword Creation
Wizard".

The "Analysis detail" section also provides a breakdown of the different
structure types. Here, you can see the number of schools, churches or
government buildings that are affected or not affected. Using the map
canvas, you can then identify where those buildings are, to assist
with planning a response to such an event.

.. figure:: /images/001_basic_pacsafe_analysis_detail.png
   :align: center

   Analysis detail table for tsunami inundation impact.

The "Action checklist" section provides some leading questions that
may need to be answered by emergency managers. These questions are
intended to be addressed *before* a disaster, in preparing response
plans. The list of questions can also be customised to suit different
agencies and their role in managing a disaster response.


The "Aggregation result" section provides a summary of the number of
buildings in each aggregation area that are affected by the
tsunami. In this scenario, we have not performed any aggregation, so
the report only shows two rows - "Entire area" and "Total" - which
both contain the same values.

.. figure:: /images/001_basic_pacsafe_aggregation_result.png
   :align: center

   Aggregation result for the first tsunami inundation scenario, where
   no aggregation is performed.

In the next session, we will show you how to run |project_name|
analyses with aggregation.


.. _print-save:

Print and Save your |project_name| Results
..........................................

We can also print the analysis results; the impact map and the impact
summary, as two separate pdf files. |project_name| has standard
templates for printing the maps, making it simple to generate the
reports. To print |project_name| result:

1. Click :guilabel:`Print` at the bottom of the |project_name| panel.

.. image::/images/001_basic_pacsafe_print_report.png
   :align: center

2. Almost instantly, three new PDF documents will open, each
   displaying the contents of the analysis in different formats.

a. A landscape layout map of the impact analysis area.
b. A portrait layout map of the impact analysis area.
c. A PDF version of the analysis report displayed in the |project_name| dock.

Take a look at each of the PDF documents and check the content is
similar to what you see on the map panel and in the |project_name|
dock. You can now save these to a location of your choosing, or print
them off for distribution.

For more information about printing, click :guilabel:`Help` in the
print window.

.. image:: /images/001_basic_pacsafe_landscape_map_report.png
   :align: center
   :width: 500 pt

.. image:: /images/001_impact_summary_tsunami_buildings.png
   :align: center
   :width: 300 pt

We already have the impact result in pdf files, but what if we
want to keep the impact result in shapefile? Is the impact result
shapefile automatically stored?

The |project_name| impact result layer is saved in a temporary folder,
this means that it will be automatically deleted if you restart your
computer, unless you save your |project_name| project. If you want to
keep your |project_name| results (so you can refer to them again or
share them with others), you need to manually save the |project_name|
impact layer |project_name| as new layer in same directory as your
project.

1. Right click on your |project_name| analysis result, for example **Number of Buildings** or **population which need evacuation**
   and click :guilabel:`Save As...`

2. A new window will appear. Click :guilabel:`Browse...` and name your
   new layer and click :guilabel:`Save` and then click :guilabel:`OK`.

If you want to save your current project you can save it by clicking
on :menuselection:`Project > Save As...` to save your current
project. It’s better to not overwrite the training project so you can
do the exercise again later.


Run |project_name| analysis for population
------------------------------------------

Return to the |project_name| toolbar and click on the |project_name|
button to open the project selection window. This time, select the
"Nukualofa tsunami population" project in the list, then click the
:guilabel:`Load` button. As before, the |project_name| dock should
show you are ready to run a new tsunami analysis. This time, it poses
the question "in the event of **a tsunami generated by a Mw 8.7 earthquake**, how many **people** might **be affected**?"

Click the :guilabel:`Run` button in the lower right corner of the
|project_name| dock to start the analysis process. After a few
seconds, you should get a result in the dock area, and several new
layers should be added to the map. You will see these new layers
listed in the layers panel.


Changing the analysis threshold
-------------------------------

We mentioned earlier that a disaster manager may decide that buildings
are affected if they are inundated by more than 50 cm of water. The
original analysis indicated that buildings were considered "affected"
if the inundation depth was 1.0 m or greater.

Let's return to the "Nukualofa tsunami buildings" project, and modify
the classification to change the "affected" threshold from 1.0 m to
0.5 m.

From the |project_name| toolbar, click on the |project_name| button to
open the project selection window. Select the "Nukualofa tsunami
buildings" project from the list, then click the :guilabel:`Load`
button. Because the keywords are all presently defined for this
project, the |project_name| dock will show you are ready to run a
tsunami analysis.

But we want to change the default threshold for affected buildings. To
do so, we need to update the keywords for the "Tsunami from Mw 8.7
earthquake". Select this layer in the Layers panel, then click the
**Keyword Creation Wizard** button in the |project_name| toolbar.

.. image:: /images/Intro_QGIS_39.png
   :align: center

This will open the **Keyword Creation Wizard** window.

.. image:: /images/001_basic_pacsafe_keywords_001.png
   :align: center

Through the wizard, you can define the keywords that describe the data
layer. In this case, the keywords are already defined, and the wizard
will show the current values for the "Tsunami" layer. On the first
screen, you can select the purpose of the layer, which for the
"Tsunami" layer is a "Hazard" layer. The "Hazard" option is already
selected, so you need only click :guilabel:`Next` to confirm this
option.

Next is to define the type of hazard. The layer has previously been
defined as a "Tsunami" layer, so this option will be selected in the
list of hazards. Again, click :guilabel:`Next` to confirm the selection.

.. image:: /images/001_basic_pacsafe_keywords_002.png
   :align: center

The "Tsunami" layer represents the inundation from a single tsunami
event (see the :ref:`|project_name| concepts <single_vs_multiple>`
section), so we select the "Single event" option to describe the
**hazard scenario**. Click :guilabel:`Next` to confirm.

.. image:: /images/001_basic_pacsafe_keywords_003.png
   :align: center

The next screen asks you to select whether the data is
:ref:`continuous or classified <continuous_vs_classified>`. The data
here represent a continuous layer, so again we click :guilabel:`Next`
to confirm and move to the next screen.

.. image:: /images/001_basic_pacsafe_keywords_004.png
   :align: center

Now we confirm the units of the tsunami hazard layer. Different hazard
layers will have different units options. In the case of tsunami,
there are only two options: **feet** and **metres**. Our hazard data
is in units of metres, which is already selected. Click
:guilabel:`Next` to confirm and move to the next step.

.. image:: /images/001_basic_pacsafe_keywords_005.png
   :align: center

We have now reached the step where we select the classifications for
our hazard data. |project_name| allows you to set different
classifications for different exposure types - land cover, population,
roads and buildings. In this project, we are analysing the impacts of
tsunami on buildings, so we want to edit the **Tsunami on Structures
Classification**.

.. image:: /images/001_basic_pacsafe_keywords_006.png
   :align: center

Here, you can see that the **Tsunami on Structures Classification** is
set to "Tsunami classes", and the :guilabel:`Edit` button is
active. On the right, you can see that under the **Tsunami on
Structures Classification** there are some values set in the
table. Now click the :guilabel:`Edit` button.

.. image:: /images/001_basic_pacsafe_keywords_007.png
   :align: center

You can now change the values against each class of hazard zone. 

Remember back to the Impact Summary report, where those structures in
a **Low Hazard Zone** were considered unaffected. If, as a disaster
manager, you want to change the threshold of affected buildings to 50
cm, then you would change the :guilabel:`Max` value for the **Low
hazard zone** to a value of :samp:`0.50`. This will automatically
change the :guilabel:`Min` threshold for the **Medium hazard zone** to
:samp:`0.50`.

.. image:: /images/001_basic_pacsafe_keywords_008.png
   :align: center

Click the :guilabel:`Save` button to save the new values. Now click
:guilabel:`Next` to confirm the changes and move to the next step of
the **Keyword Creation Wizard**.

On this screen, you can make notes on the source of the data. For now,
we will leave these as they are set. Click :guilabel:`Next`, where we
can set a title for the layer. Again, we will leave this
unchanged. Click :guilabel:`Next` one more time.

.. image:: /images/001_basic_pacsafe_keywords_009.png
   :align: center

On this last screen, you can review the keywords and classifications
that you have set. Check to make sure the classification for **Low
hazard zone** has a maximum value of :samp:`0.5`.

If you want to make further changes, simply click the :guilabel:`Back`
button until you reach the screen you want to change. Otherwise, click
:guilabel:`Finish`. We are now ready to run the analysis again, with
the new threshold of 0.5 m.

Make sure the **Tsunami from Mw8.7 earthquake** layer is selected in
the Layers panel, then the |project_name| dock should show you are
ready to run an analysis. Click the :guilabel:`Run` button to start
the analysis.

A new impact layer will be added to the Layers panel, which contains
the results of the new analysis.

Look at the Impact Summary report, and compare it to the previous
Summary report you produced. Have the number of buildings changed in
the "Affected" and "Not affected" columns? What might this mean for
response actions?



Summary
-------

In this exercise you have learned how to run a basic |project_name|
analysis using an existing |project_name| project file and what the
minimums component that must be there to run |project_name| properly
are. Those components are hazard and exposure data. In this exercise,
you have run an |project_name| impact assessment for a tsunami
scenario in Nuku'alofa using two types of exposure data. The hazard
data you used was a modelled tsunami raster and the exposure data were
buildings and population. These analyses produced impact layers and
impact summaries for affected buildings and impacted people.

You have also learned how to modify the analysis options through the
Impact Function configuration, how to print |project_name| results in PDF
format, understand what minimum needs is and how to save both your
impact layers and your |project_name| project file.

In the next section you will learn more about how to run
|project_name| in more detail. In that module you will learn how to
use more |project_name| tools such as Agreggation options, OSM
Downloader, Minimum Needs Configuration, etc.









