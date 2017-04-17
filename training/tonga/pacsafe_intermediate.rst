.. image:: /images/pacsafe.png

.. _intermediate-pacsafe:

Run intermediate |project_name|
===============================


Introduction
------------

In :ref:`basic-pacsafe`, we learned how to run a tsunami inundation
analysis on population and buildings, adjust the tsunami impact
default settings and analyze the impact summary report. We also
learned how to save the analysis data and generate a PDF of the
analysis results.

In this exercise, we will learn more techniques such as how to run
|project_name| with aggregation data to produce reports broken down by
districts or villages. We will also learn how to define the analysis
area, so we can examine a smaller region.

Learning Objective
..................

To improve the participant's understanding of additional
|project_name| function and features. By the end of this exercise,
participants will be able to:

* Define keywords using the |project_name| keyword wizard
* Run |project_name| with aggregation data
* Set the |project_name| analysis area using the |project_name|
  analysis area tool.

Exercise
--------

We will assume here that you can start the |project_name| application
and opent the project selection menu.

Run |project_name| for Tropical Cyclone Wind
............................................

Click the :guilabel:`PacSAFE` icon and select the "Nukualofa Tropical
Cyclone buildings" project, then click the :guilabel:`Load` button.

As with the previous exercise, this project will show several layers:

* Buildings: the exposure data, the same as the previous exercise.
* Tropical cyclone: a wind field from a simulated tropical cyclone.
* Imagery: aerial imagery to provide contextual information.


Run |project_name| analysis for buildings
-----------------------------------------

In the |project_name| dock on the right, 


Define keyword for hazard data
..............................

|project_name| need a keyword to determine what type of data the user
provide for analysis (hazard data, exposure data or aggregation data).
If the data provided does not have a keyword, it will show a warning
message “Layer Keyword Missing” in the |project_name| dock. Try
selecting :guilabel:`A cetegory 3 cyclone in Tongatapu` layer and look
at the |project_name| dock, You will see the following:

.. image:: /static/training/socialisation/intermediate_inasafe_03.*
   :align: center
   :width: 300 pt

As you can see from the picture above, this layer keywords are missing
and we need to open the keyword wizard to solve this problem. The
keywords wizard will take you through a step-by-step process of
assigning keywords to your data.


Select **A category 3 cyclone in Tongatapu** layer and click
:guilabel:`Keyword Creation Wizard`. A window will appear and follow
the steps provided by the :guilabel:`Keyword Creation Wizard`. If you
get stuck, you can follow the diagram below to understand the steps
and the choices you will be offered.

Steps in the Keyword Creation Wizard
....................................

Starting at the top of the diagram and working down; in the first step
you will choose if your data are hazard, exposure or aggregation data.
Your choice will determine the next options offered. 
You can always go back and change things later.

If you choose Hazard or Exposure, you will need to select the type of
hazard or exposure. Next, you will choose whether the layer mode
is continuous or classified (if you forget what Continuous
or Classified means, you can reference the :ref:`pacsafe_concepts` section).
Both Hazard and Exposure types have the same step after you define the
layer mode: defining which unit or attribute represents the hazard. 

The steps will be different for aggregation data. After you define the
data as aggregation data, you will select the attribute to represent
the names of aggregation areas. After you select it, you will be asked
to define the population ratio. Finally, you will need to enter the
source of data and the name of your layer to be displayed in the
|project_name| dock.

.. image:: /static/training/socialisation/intermediate_inasafe_04.*
   :align: center
   :width: 300 pt

.. image:: /static/training/socialisation/intermediate_inasafe_05.*
   :align: center
   :width: 300 pt

After you set the keyword using the Keyword Wizard, you can see in the
|project_name| panel on the right side that the layer keyword has been
set.  Verify that it looks like the image below? If it does not, you
should go back and try to define the keyword again.

.. image:: /static/training/socialisation/intermediate_inasafe_06.*
   :align: center
   :width: 300 pt

After you set the keyword to match the image above, the hazard data will
appear in the hazard panel of the |project_name| Dock.

.. image:: /static/training/socialisation/intermediate_inasafe_07.*
   :align: center
   :width: 300 pt

Now all the keyword data has been set and we can move into the next
section to run |project_name| with population data.

Run |project_name| for buildings with aggregation
-------------------------------------------------

We have seen the result of |project_name| on buildings and populations
with raster hazard data. Now we will run |project_name| analysis using
cyclone raster hazard data and vector buildings as exposure data. This
time, however, we will use aggregated data. Using |project_name| with
aggregated data will help you to get detailed result since the
aggregated data can provide detailed information on specific
administrative (or other) area. |project_name| allow us to add
administrative data with specific boundaries that we can use to
aggregate results.

To do this, look at the Layer List and make sure to turn ON the
**Tonga districts** layer. Next, take a look at the |project_name|
dock under the heading *Aggregate results by*.

.. image:: /static/training/socialisation/intermediate_inasafe_08.*
   :align: center
   :width: 300 pt

Why are we not able to see the **Tonga Districts** layer that we just
turned ON before? Check the layer by selecting it on the Layer
List. Did you see the keyword? The reason why this layer did not
appear in the |project_name| Dock is because it did not have keyword
data defined. Go ahead and add a keyword for **Tonga Districts** using
the :guilabel:`Keyword Creation Wizard`. For your reference, refer to
the keyword diagram as explained above.

Now you will able to select **Tonga Districts** under 'Aggregate
results by' in the |project_name| Dock. The |project_name| Dock should
look like this:

.. image:: /static/training/socialisation/intermediate_inasafe_09.*
   :align: center
   :width: 300 pt

Click :guilabel:`Run` and wait until |project_name| finishes analyzing
the data. A new impact layer will be added to the Layer List. When you
look at the result, it looks the same as |project_name| analysis
result without aggregation, but if you scroll down to the bottom you
will see the detailed result. As explained before, using aggregation
will let you get detailed information for a specific area or
administration region.

.. image:: /static/training/socialisation/intermediate_inasafe_10.*
   :align: center
   :width: 300 pt

In the screenshot above, we see detailed impact results for each
district in Tongatapu building report.  The aggregation option in
|project_name| can also be applied for population and roads (in
addition to buildings).


Define your custom analysis area
--------------------------------

|project_name| has a feature that allows you specify exactly which
area should be used for your analysis. If you have exposure data that
is not the same size as the hazard layer, you can use this feature to
define your own analysis area.

1. Click :guilabel:`Set Analysis Area` to show set analysis extent feature.

2. Select :guilabel:`Use intersection of hazard, exposure and this bounding box`.

3. Click :guilabel:`Drag on Map` to draw the bounding box around
   building polygons and roads.

4. Click :guilabel:`OK`

.. note:: if you click Draw on Map, the window will be temporarily hidden
          so that you can drag a rectangle on the map. After you have finished
	  dragging the rectangle, the window will reappear.

.. image:: /static/training/socialisation/intermediate_inasafe_12.*
   :align: center
   :width: 300 pt

To verify that your analysis area has been successfully defined, click
:guilabel:`Toggle Scenario Outlines`. A green box will appear around
your data.

.. image:: /static/training/socialisation/intermediate_inasafe_13.*
   :align: center
   :width: 300 pt

.. note:: Using Toggle Scenario Outlines help you understand which
          area that |project_name| will analyze. It is also an important
          step before running |project_name| analysis because not all of
          the data you put in the Layer List will be automatically
          defined by |project_name|.

Take a look at the |project_name| panel dock to make sure building
polygons and roads have a keyword defined. If they do not you can
define one using :guilabel:`PacSAFE Keyword Wizard`.

After the keyword has been already set, we are ready to run
|project_name| for building polygons and roads.

Run |project_name| analysis for building points
-----------------------------------------------

Let us run analysis for building polygons first. Make sure you set the
|project_name| dock as pictured below:

.. image:: /static/training/socialisation/intermediate_inasafe_14.*
   :align: center
   :width: 300 pt

We will run |project_name| for wind raster hazard and building points
with data aggregated by Tonga village boundaries. Click
:guilabel:`Run` to begin |project_name| analysis. After running, you
will find the impact result layer in Layer List.

.. image:: /static/training/socialisation/intermediate_inasafe_15.*
   :align: center
   :width: 300 pt

Looking at the **Detailed building type report** (pictured above) we
only see two districts in Nuku'alofa. Your results may differ since it
depend on the analysis area selected and also the aggregation layer
that you used for analysis.

Summary
-------

In this exercise, you have learned how to run |project_name| analysis
with different hazard data formats and with new type of exposure
data. You have also learned two fundamental steps to remember before
you run |project_name|:

First, you learned how to define a keyword for your data so it can be
analyzed with |project_name|. Without a keyword, |project_name| will
not recognize your data, so you need to define it whether the data is
hazard, exposure or aggregation data. You can set the keyword using
the :guilabel:`Keyword Creation Wizard` feature.

Second, it is important to review the analysis area using *Toggle
Scenario Outline* before you run |project_name| analysis. This is
because, |project_name| sometimes does not automatically set the
analysis area according to the intersection of hazard and exposure
data. If |project_name| did not set the analysis area, you need to
define it manually using the :guilabel:`Set Analysis Area` feature.

In the next section, you will learn how to run |project_name| with
other type of hazard data such as tsunami, earthquake, volcano and
generic data.
