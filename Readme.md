# Roll Samples

### Example projects for the QGIS Seismic survey design plugin 'Roll"'

#### 1	Introduction

This repository contains a number of example projects for '**Roll**'. Several templates are shown in these sample files:

- Brick
- Parallel
- Double zigzag
- Triple zigzag
- circles
- spirals
- wells

The templates that are using  **well** based seed  are referring to external "**well files**"

These are ascii files for which two formats are currently supported:

- *.well	OpendTect (x, y, z) format

- *.wws	GeoPath (ahd, inc, azi) format 



#### 2	Well File locations

At the moment, the **well files** are referred to using 'absolute paths' instead of 'relative paths'

This means that you'll have to update the location of the well files, when using the examples:

- Wells-well.roll
- Wells2-well.roll
- Wells-wws.roll



#### 3	Circles and Spirals

The above listed projects not only contain well-based seeds but also some circle and spiral based seeds, that may be used when acquiring a VSP



