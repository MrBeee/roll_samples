# Roll Samples

### Example projects for the QGIS Seismic survey design plugin 'Roll'

#### 1	Introduction

This repository contains a number of example projects for '**Roll**'. Several templates are shown in these sample files:

- Brick
- Parallel
- Double zigzag
- Triple zigzag
- circles
- spirals
- wells



#### 2	Well based seeds

The templates that are using  **well based seeds**  are referring to external "**well files**"

These are ascii files for which two formats are currently supported:

- ***.wws**	GeoPath (ahd, inc, azi) deviation format 
- ***.well**	OpendTect (x, y, z) format

The **GeoPath** (ahd, inc, azi) deviation is resampled to local (x, y, z) values for specified along-hole positions using the minimum curvature approach. 

The **OpendTect** (x, y, z) format is first converted into a deviation format, before resampling specified along-hole positions to local (x, y, z) values, using the minimum curvature approach. This minimizes position errors related to a curved well trajectory.



#### 3	Well File locations

At the moment, the **well files** are imported using 'absolute paths' instead of 'relative paths'. This means that you'll have to update the location of the well files, when using the following examples for the first time:

- Wells-well.roll
- Wells2-well.roll
- Wells-wws.roll



#### 4	Circles and Spirals

The  three projects listed above, not only contain well-based seeds but also some **circle** and **spiral** based seeds, that may be used when acquiring a VSP


