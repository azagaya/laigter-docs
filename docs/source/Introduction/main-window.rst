Laigter's Main Window
=====================

I try to keep Laigter's GUI as simple as possible, with all needed controls at reach.
For this, the main window is made with a central widget, where all the rendering
happens, and movable dock widgets, with the controls needed to tweak the maps.
Also, there is a toolbar with buttons for the most used features of the tool.
When opening Laigter, you should see this window:

.. image:: img/MainWindow.png

Toolbar buttons
---------------
In the toolbar, you will notice a few buttons. This is a brief explanation of each
one, in order of appearance in the GUI:

- |open| Open Project: Open a previously saved Laigter project file.
- |save| Save Project: Save current work as a Laigter project file. If the project has not been saved previously, it will trigger *Save As* instead.

- |save-as| Save As: Saves current work as a new Laigter project. A dialog will pop up and let you choose the location and name of the file.

- |import| Import: Opens a dialog to choose images to import in Laigter's current project.

- |fit-zoom| Fit Zoom: Applies the right amount of zoom and translation of the canvas, in order to fit all textures in the current view.

- |100-zoom| Zoom 100%: Restores the default zoom (1:1 scale of the textures).
- |zoom+| Zoom +: Zooms in the canvas.
- |zoom-| Zoom -: Zooms out the canvas.

- |export| Export: Exports the maps of the currently selected texture. A dialog will let you choose the location and base name for the maps. Selecting which maps to export and batch exporting will be expanded on other sections.

- |add-light| Add Light: While on preview mode, it lets you add or remove light sources. Will be covered in other sections.

- |presets| Presets: Lets you save/load/apply presets to the selected textures. Will be covered in other sections.

- Language: Lets you select the language of your preference for the GUI.

- |about| About: Opens a window with information about Laigter version, contributors, supporters, links to relevant sites, etc.

- |themes| Theme: Lets you select the theme for the GUI.
- |add-plugin| Install Plugin: Opens a dialog to select a plugin from your file system and install it to Laigter.

- |remove-plugin| Delete Plugin: Opens a dialog to select and delete a specific plugin.

- |reload-plugin| Reload Plugin: Reload all installed plugins.

Dock Widgets
------------

Most of the controls of Laigter are placed in dock widgets that you can move around the GUI. The following image shows all of the dock widgets together:

.. image:: img/DockWidgets.png

The controls of each individual dock widget will be explained in a section of their own, but here is a brief explanation of the docks.

- Normal/Specular/Parallax/Occlusion: this dock contains the controls for tweaking the generation of each map.
- Sprite Properties Dock Widget: In this dock, you have some controls and information of the currently selected sprite. You can change its position in the canvas, as well as its rotation and scale. You can select to generate maps in a *tiled* way, and choose how to extend it outside it bonds (select neighbors). Also, here you can make animations out of a sprite sheet, splitting the texture in multiple frames.
- Visualization: This dock lets you choose what map you want to see, or select preview to see the result with dynamic lighting. Also, some other controls let you tweak the preview a bit.
- Textures: This dock just contains a list of the currently opened textures. You can select multiple of them to show them all at the same time in the central widget.
- Export: In this dock, you can select which maps you want to export, and if you want to export directly in the location of the original sprite (Export button) or to a specified folder (Export to.. button). This makes a batch export, exporting maps of all textures.

Sliders
-------

Almost all controls in Laigter's gui are standard, so no explanation is required to use them. However, the slider in Laigter is a custom widget, so a brief usage explanation may be useful.

A slider in Laigter looks like this:

.. image:: img/Slider.png

The usage is simple: you can grab it from the right little square indicator, or you can simply write a number, and the slider value will be updated. And that's all!

.. |open| image:: img/open.png
          :scale: 50 %
.. |save| image:: img/save.png
          :scale: 50 %
.. |save-as| image:: img/save_as.png
             :scale: 50 %
.. |import| image:: img/import.png
            :scale: 50 %
.. |fit-zoom| image:: img/zoom_fit.png
              :scale: 50 %
.. |100-zoom| image:: img/zoom100.png
              :scale: 50 %
.. |zoom+| image:: img/zoom+.png
           :scale: 50 %
.. |zoom-| image:: img/zoom-.png
           :scale: 50 %
.. |export| image:: img/export.png
            :scale: 50 %
.. |add-light| image:: img/add_light.png
               :scale: 50 %
.. |presets| image:: img/presets.png
             :scale: 50 %
.. |about| image:: img/info.png
           :scale: 50 %
.. |themes| image:: img/theme-selector.png
            :scale: 50 %
.. |add-plugin| image:: img/plugin-install.png
                :scale: 50 %
.. |remove-plugin| image:: img/plugin-delete.png
                   :scale: 50 %
.. |reload-plugin| image:: img/plugin-reload.png
                   :scale: 50 %
