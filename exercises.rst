Exercises
=========

Getting PacSAFE
---------------

Installing PacSAFE
------------------


Understanding the PacSAFE interface
-----------------------------------
There are four elements in the PacSAFE interface:

.. image:: /images/pacsafe_interface.png
   :align: center
1. **Layers panel**: On the left side of PacSAFE is the layers panel. This panel lists the layers, or files, that are loaded into our PacSAFE project. The Layers Panel not only shows all the files that are currently open, it also determines the order that they will be drawn on the map canvas. A layer that is at the bottom of the list will be drawn first, and any layers above it will be drawn on top.
2. **Toolbar**: At the top of PacSAFE are a large number of tools, which are contained within various toolbars. For example, the File toolbar allows you to save, load, print and start a new project. We already used one of these tools when we opened this project. By hovering your mouse over an icon, the name of the tool will appear to help you identify each tool. The number of tools (buttons) can seem a bit overwhelming at first, but you will gradually get to know them. The tools are grouped into related functions on toolbars. If you look closely you can see a vertical array of ten dots to the left of each toolbar. By grabbing these with your mouse, you can move the toolbar to a more convenient location, or separate it so that it sits on its own.


3. **Map canvas**: All of the map data that we load into PacSAFE will be displayed here, both vector data and raster data.
4. **PacSAFE dock**: After successfully opening PacSAFE, you should have a **PacSAFE dock** on the right hand side of the screen. It should look like this:


PacSAFE basic tools
-------------------

We’ve already taken a look at the QGIS toolbar and have seen the tools for opening QGIS. Here's a list of some of the most commonly used tools. Feel free to play around with them if you like. The important thing for now is to start getting familiar with QGIS.


Navigating the map
------------------

Before we examine the attributes of individual features, let’s take a quick look at how to navigate the map. The main controls for moving the map around and zooming in-and-out are on the panels at the top of QGIS by default.

.. image:: /images/map_navigation.png
   :align: center

When you click on one of these buttons, it changes the action of the mouse in the main map window.

* Select the first button that looks like a hand. Now hold the left mouse button down and drag the mouse in the map window. This allows you to **pan** the map, or move it around.
* Selecting the button that has a plus sign (+) inside a magnifying glass allows you to **zoom in** on the map. Using your mouse, draw a boz around your area of interest and release your mouse.
* Selecting the button with a minus sign (-) inside a magnifying glass allows you to **zoom out** on the map. Select this button and click on the map.
* The button that looks like a magnifying glass with blue arrows pointing away from it lets you **zoom to the full extent** of your map. Click this button to see all the data that is loaded in the project fit into the map canvas.



Hide and move layers
--------------------

Sometimes if you handle many layers, you need to hide/unhide layers to make the map canvas more organized. For example, open the pre-saved QGIS project, DKI_Jakarta_Introduction.qgs. Once all the data are displayed on your map canvas, try toggling the layer, **a flood similar to the 2007 Jakarta Event** by clicking on the checkbox in the Layers Panel on the left side of your screen.



After you uncheck the check box, the layer will disappear from the map canvas. This operation won't remove your layer from the layers list but only hide it temporarily until you recheck again the check box. Try to turn ON the layer again to unhide the layer.

What if your layer does not appear in the map canvas even though you already turned ON your layers? In this example, the **Jakarta_roads_WGS84** layer didn’t appear in Map Canvas even though it's already turned ON. In this case, it's related to layer order. The layers in your Layers List are drawn on the map in a certain order. The layer at the bottom of the list is drawn first, and the layer at the top is drawn last. By changing the order of the layers in the list, you can change the order they are drawn in.

Symbolize a layer
-----------------

PacSAFE toolbar
---------------

PacSAFE also comes with a toolbar of it's own! To retrieve the PacSAFE toolbar, you can right-click on the top toolbar and check **PacSAFE**.

Summary
-------

In this exercise you have learned about QGIS, the free and open source software for processing spatial data. You have learned where to get QGIS, how to install QGIS, understand the QGIS layout and looked at some useful toolbars, learning how to turn ON/OFF QGIS layers, and learned how to symbolize the data layers.

