Normal Map Generation
=====================

Laigter aims to be a simple normal map generator. To tweak the normal map you only
to play arround with the sliders until you get the desired result. In this section
what each of those sliders do will be explained.

Al the controls that affect the normal map generation are grouped under the **Normal**
dock widget. 

Enhance controls
----------------

The controls under this group affect the detail, or *inner regions* of the sprite.
For better understanding of what they do, lets put the controls under *Bump* group
to zero.

There are just two controls under the *Enhance* group, *Height* and *Soft*.

Height Control
""""""""""""""

A normal vector can be thought as the derivative of the height on a surface. If
that height almost doesn't change (like on a flat surface) the normal will point
upwards (or to the screen, in our case of 2D textures). This will lead to the blueish
color we talked about in the :ref:`intro:What are normal maps?` section.
