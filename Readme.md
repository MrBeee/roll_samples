# Roll Samples

### Example projects for the QGIS Seismic survey design plugin 'Roll'

#### 1	Introduction

This repository contains a number of example projects for '**Roll**'. Several basic geometries are shown in these sample files:

- Brick
- Parallel
- Double zigzag
- Triple zigzag
- wells (*in conjunction with circles and spirals*)
- Noordoostpolder (*a fully worked out example showing interaction with QGIS*)



#### 2	Well based seeds

The templates that are using  **well based seeds**  are referring to external "**well files**"

These are ascii files for which two formats are currently supported:

- ***.wws**	GeoPath (ahd, inc, azi) deviation format 
- ***.well**	OpendTect (x, y, z) format

The **GeoPath** (ahd, inc, azi) deviation trajectory is resampled to local (x, y, z) values for specified along-hole positions using the minimum curvature approach. 

The **OpendTect** (x, y, z) format is first converted into a deviation format, before resampling specified along-hole positions to local (x, y, z) values, using the minimum curvature approach. This minimizes position errors related to a curved well trajectory.



#### 3	Well File locations

At the moment, the **well files** are imported using 'absolute paths' instead of 'relative paths'. This means that you'll have to update the location of the well files, when using the following examples for the first time:

- Wells-well.roll   (This sample uses wells in the *.well format)
- Wells-wws.roll  (This sample uses wells in the *.wws format)



#### 4	Circles and Spirals

The  wells projects listed above, not only contain well-based seeds but also contain some **circle** and **spiral** based seeds, that may be used when acquiring a 3D VSP



#### 5	Noordoostpolder example

This example starts with defining an orthogonal template that is converted into geometry files, which are then exported to QGIS for further editing (enabling / disabling / deletion / move around). Once editing is completed, the points are re-imported into Roll for analysis of the fold map, as well as minimum- / maximum offset charts. These figures can then be exported to QGIS as georeferenced tiff files, so the results of the edits are displayed in QGIS itself.

