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
color we talked about in the `normal map example <https://laigter.readthedocs.io/en/latest/Introduction/intro.html#normal-map-example>`_ of the introduction section.
So thiscontrol lets you chose how high is the difference in height between
consecutive pixels. A lower value then, will result in a more flat normal map
(more blueish).
A higher value would mean normal vector directions point to other directions,
and so, more *colorful* normal map (as colors represent components of the vector).
The effect of the light will be more noticeable in this last case.

.. figure:: img/enhance-height-map.gif

   Effect of *Enhance* height control in the normal map.

.. figure:: img/enhance-height-preview.gif

   Effect of the *Enhance* height control in the preview.

Soft Control
""""""""""""

After the normal map due to the enhance controls was generated, a blur is applied
to get a better looking result. The ammount of blur applied is controller with this
slider.

.. figure:: img/enhance-soft-map.gif

   Effect of *Enhance* soft control in the normal map.

.. figure:: img/enchance-soft-preview.gif

   Effect of the *Enhance* soft control in the preview.

Bump controls
-------------

Enhance controls are meant for generating normals of inner details of the texture.
But for 2D sprite, is usefull to give some bump effect from its edges. This means,
make the sprite look like it has volume. For this we use the controls under the
*Bump* group.


