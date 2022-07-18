---
title: "Middle of Nowhere Render"
date: 2022-07-06T10:50:48-07:00
draft: false
tags: ['images','cartooon']
---
Render of the house/farm from the cartoon Courage
the Cowardly Dog

![Courage render](/couragerender.webp)

Ground texture was a real life photo taken from the Painted Hills
in Oregon. 
![Painted hills](/paintedhills.jpg)
![Rock texture full](/origfloor.jpg)

I turned that picture into a seamless 256x256 texture for
use in this scene

![Ground texture](/crackedrock.png)

Roof texture was made with a noise texture and then stretching
and coloring that noise texture with a color ramp to look like a wood grain.

# Material Breakdown
![Wood breakdown](/breakdown.gif)

House uses the same wood material with different colors and then adds a brick texture
over the material.

![Brick House](/brickhouse.png)

Then to not have that brick texture at all parts of the house a musgrave texture is 
used to mask the brick house.

![House musgrave mask](/housemask.png)

All together

![Complete house material](/compdhouse.png)

Reference image from the show

![Reference](/courageref.jpeg)
