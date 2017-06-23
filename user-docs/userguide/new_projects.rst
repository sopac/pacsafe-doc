.. _new_projects:

Adding new projects to |project_name|
=====================================

Users can add new QGIS projects to the list of projects for use in
|project_name|

Use the :guilabel:`pacsafe-advanced.bat` version to create your
project, as this will allow you to update elements such as the project
title and ensure the project uses relative paths.

Follow these guidelines to add your own projects:

1. Projects should be named with underscores :samp:`_` instead of
   spaces. Set the name to something meanigful, so other people might
   understand what the project comprises
2. All data should be stored under subdirectories where the project is
   saved. Currently, there are a limited number of subfolders, to make
   maintaining the data easier. New exposure data should be stored
   under the :file:`exposure` folder, :file:`raster` holds the raster
   hazard layers, :file:`imagery` stores the satellite imagery used for
   context in the projects.
3. Make sure the project stores the path to the data layers as
   *relative paths*.  Go to :menuselection:`Project --> Project
   properties --> General settings --> Save paths` and ensure it is
   set to "relative".
4. Set the title of the project to something meaningful, so other
   people might understand what the project comprises:
   :menuselection:`Project --> Project properties --> General settings
   --> Project title`
5. Copy the project file, and any additional data, to the
   :file:`data/to` folder (for Tonga projects).

When you next start |project_name|, your project should appear in the
Project Selection window.
