---
title: "Pyramid Render"
date: 2022-07-17T21:11:03-07:00
tags: ["images"]
---
Render of pyramid environment

![Dawn Pyramid](/pyramiddawn.png)


Render of mars-like desert pyramid.
![Mars pyramid](/marspyramid.png)


# Material Breakdown

Here I used the ocean modifer to create the dunes

![desert wireframe](/desertwireframe.png)

Then I created a color ramp based on the height of the dunes

![desert colorramp](/desertcoloramp.png)

Sandlines were generated using the wave texture node, which looks very similar
to the sandlines I am trying to replicate.
This colorramp was then used to control the "waveiness" of the sand lines, 
which is something I noticed happening in real dunes when looking for reference images.

![desert wave](/desertwaveinvert.png)

This wave was then combined with a noise map to add a little more texture for the sand grains. All of that was fed into a normal map which is something the renderer can
use to fake more complex models. The normal map tells the renderer what way a given face
is pointing in order to make somewhat convincing depth.

![desert normal map](/desertnormalmap.png)

This gif illustrates what normal maps are doing, the left being modeled shapes, and
the right being normals maps generated from the models on  the left. This shows
how you can fake geometry with normal maps. Normal maps are very useful for speeding
up the rendering of complex scenes. For example, Video Game graphics where many 
frames need to be rendered every second.

![normal map gif](/normalmap.gif)

When all is combined with a sand color, this is what we get.

![Final desert](/finaldesert.png)
