Parallax Map Generation
=======================

This one is probably the less used map in 2D games, but you can generate and preview
it with Laigter anyways! Parallax mapping is similar to displacement techniques, in
the sense that both techniques use gray scale textures to give information about
height/depth/displacement. In displacement techniques, however, we use that
information to move the vertices of the 3D object to achieve better surface detail.
This makes it necessary for the object to have many vertices to look nice.
Parallax mapping, instead, makes the calculation on fragments, just picking the color
the user would see if the object had that displacement. This way, we can just apply
the displacement with as little as four vertices (one quad or two triangles).

This is an example of how a 2D texture looks with parallax mapping technique.

.. figure:: img/example-parallax.gif

   Parallax effect example.

Parallax generation in Laigter has two modes, *Binary* and *Heightmap*. The first
makes a black and white version of the current texture, and lets you adjust some
parameters to tweak the parallax map. The resulting parallax map is still a
gray scale image, as the controls will affect the resulting color. The latter will
take the generated heightmap for normal map calculation, and use it directly as a
parallax map, again, allowing user to tewak it through controls.

.. note::
   In Laigter, the parallax map is analogue to a depth map. Lighter colors mean
   that fragment should be at deeper z position, and darker colors means the fragment
   should remain closer to  the original position. Of course, the z position is just
   an effect, as no 3D processing is done here.

Binary Mode
-----------

Binary mode is useful for simple patrons, like brick walls. It will binarize an image
given a threshold, and generate the parallax map from that image.

.. note::
   For those who doesn't know, binarizeing an image means taking the value of a pixel,
   and making it white if its above a threshold, or black if its below.

Threshold Control
-----------------

This control allows the user to chose the threshold for the binarization.

.. figure:: img/threshold-parallax.gif

   Effect of *Threshold* control on parallax map.

Focus Control
-------------

This control applies a blur previous to the binarization. That way, is the
image is to noisy, you can get rid of small "islands" when making the binary
image.

.. figure:: img/focus-parallax.gif

   Effect of *Focus* control on parallax map.
