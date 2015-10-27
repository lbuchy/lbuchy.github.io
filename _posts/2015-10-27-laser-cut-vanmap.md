---
layout: post
title:  "How to make laser cut maps"
date:   2015-10-27 14:09:04 -0700
categories: DIY woodworking
---

I find that the best way to learn something new is to just pick a project and
try to figure out how to get it done.  Yes, there will be problems along the way.
You might get half way through only to realize that you messed up at step 2 and
need to undo all your work and start again.  It can be frustrating, but I like
to think of this as part of the fun.

The purpose of this post is to document one such project that I recently finished
where I went into it without having many of the skills to do it.  I tried and failed
a few times but eventually I finished it and am fairly pleased with the results.
The project was to create a map of Vancouver which emphasises the depth of the
ocean off the coast of the city.

![Vancouver Laser Cut Map]({{ site.url }}/assets/vanmap/vanmap-top-angle.jpg)

Materials
=========
* 4'x8'x1/8" baltic birch plywood
* 1"x6"x8' red cedar
* Lighter wood stain
* Blue (Deep ocean) wood stain
* Dark (Espresso) wood stain
* Glossy varathane spray
* Wood glue
* Wood conditioner
* Wood filler
* Solvent (Mineral spirits)

Tools
=====
* Band saw
* Skill saw
* Sand paper (100 and 220 grit)
* Clamps
* Miter clamp
* Laser cutter (40W)
* Paint brush

Generating Vectors
==================

The first step is to obtain data to generate vectors representing the geography
of the area we are interested in.  This will eventually be fed into the laser
cutter and used to slice the plywood into the shapes we need.

This particular map was created using a combination of data from multiple sources.
The bathmetric data was obtained from
[Fisheries and Oceans Canada](http://www.charts.gc.ca/data-gestion/bathy/nr-rm-lic-eng.asp)
and the city data from [Open Street Map](https://www.openstreetmap.org).  To
work with this data, I imported it using [qgis](http://www.qgis.org).  Within
this program, we have the ability to combine the geographical data into a single
image and export it to .dxf.

To create the underwater contours, I found the bathymetric layer that provides
contours at 10m intervals.  This was too fine-grained for me - I would be laser
cutting a lot more than a half sheet of plywood! Therefore I separated the
contours that lay on 50m, 100m and 150m into their own layer.  This would
provide the vectors to cut the plywood.  The remaining contours would be used to
engrave the plywood.

I wanted to make sure that the land components of the map had a similar amount
of complexity.  I opted to mapping out only the arterial roads of Vancouver.
I found that the quality of data that OSM give you is pretty poor.  Most roads
were actually comprised of very small vectors that coincided with each other,
this made for really slow laser cutting and a poor finish.  I spent a lot of
time tidying the vectors in Illustrator to have long continuous lines.  I would
recommend finding data from another source next time; the City of Vancouver
seems to publish better quality data.

Building the Map
================

The physical map is comprised of five layers of plywood glued together with
ordinary woodglue and framed with 1"x1" cedar boards. All layers were stained
individually BEFORE engraving with the cutter. I want to emphasize that staining
them before is really important. If trying to do it the other way, then the
stain reduces the contrast of the engraved lines quite substantially.

Here is a photo of my first attempt. I was pretty pleased when I finished all
this cutting and pretty devastated when the stain erased a lot of the lines.

![All the layers stacked up]({{ site.url }}/assets/vanmap/vanmap-layers-unpainted.jpg)

When staining your wood, I would recommend always using wood conditioner for
softwoods(conifers) like cedar or diffuse-porous hardwoods like birch. It seems
to give you a much more uniform color with the tradeoff of making the color lighter.

The blue of the ocean was made by diluting the water-based blue stain about 20:1
water-stain ratio. The thing I would do differently next time is to be precise.
I didn't make enough stain the first time and had to make more, but I didn't
really measure anything which means some of the layers have different shades of
blue. Meh.

The land was stained with something I found in the back of my closet (no idea
what color or brand).

I opted to not varnish the blue plywood since I found it muted the blue colors
significantly. This is probably because I used water-based stain. The drawback
to this is that I expect the map to degrade quicker over time as the wood
oxidizes and the oils in people's skin eat at the wood. Oil-based stain is
probably the way to go next time. Just do a light layer though on since it needs
to be laser cut! Fumes = bad.

Once all the pieces were cut out, they were glued to each other and clamped
together.
The entire map was then glued onto a piece of laser cut plywood that was 1/2"
larger in both directions. This is used to secure the map to the frame
(more on this later)

The frame would be an optional component if you planned this properly from the
beginning since framing can be very affordable in standard sizes.
Sadly I made the map 14"x9" - not really a standard... However, I learned a
whole bunch of new skills by taking the opportunity to make my own frame!

I have a few 1"x6" sitting around at home from previous projects.
Fortunately, they were already planed and no longer warped, leaving me with a
nice surface to work with. Using the miter saw, I cut the board into the the
longest length I would need (~17") and then used the bandsaw with a fence
to cut 1" strips (table saws work well for this also). The bandsaw I used was
a bit wonky and doesn't really do a great job of making 90 degree cuts. The
blade bent a bit, however, I found the less-than-precise cuts a bit endearing
and kept the boards as they were. I then used the table router to cut a rabbet
on the inside with a depth of 1/8" and width of 1/4". This holds the map in
place via the 14.5" x 9.5" plywood piece I mentioned earlier.

[The rabbet to secure the map]({{ site.url }}/assets/vanmap/vanmap-rabbet-frame.jpg)

Finally, all miter joints were cut on the chop saw. I was a little imprecise
with everything so it took me a bit of trial and error to get everything fitting
properly. I used some wood-filler to fix up my mistakes. This may have been
because the boards were not perfectly squared (I could have used the table
saw or borrowed use of a joiner to be more precise - for next time I guess)

I then glued all the boards together at the same time, opting to use 3 miter
clamps and my hands to keep everything together. One technique that is useful
is to remember that wood is incredibly absorbent. This means that if you put
glue on the ends - a large amount of it will get absorbed by the board rather
than stick the boards together. To combat this, put glue on the ends and don't
stick them together - instead, wait 5 minutes. Pretty much all the glue will
disappear into the grain. Now put more glue on and stick them together - this
should form a much stronger bond. If you are skilled, you could also use a
biscuit cutter or cut a mortise and reinforce them with internal bracing.
External bracing is also a good option - I got lazy and did no bracing. Hasn't
broken yet, but no guarantees.

Finally, the frame was stained and finally sprayed with varathane a few times.

Below is the boards being conditioned:

![Conditioning the boards]({{ site.url }}/assets/vanmap/vanmap-frame-pieces-prestain.jpg)

Finally I added some toggles and a string to the back with some screws...

![Adding toggles and string]({{ site.url }}/assets/vanmap/vanmap-back.jpg)

... pieced it together and BOOM - project done.

![Project done]({{ site.url }}/assets/vanmap/vanmap-top.jpg)
