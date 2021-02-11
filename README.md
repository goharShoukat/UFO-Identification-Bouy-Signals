# UFO-Identification-Bouy-Signals
A C++ code for mapping out object position in the ocean from signals received from a buoy. 

There are two buoys on which radars are installed.

The two radars detected several unidentified floating objects (ofnis) in the vicinity.
When a radar detects an ofni, it provides an azimuth and an approximate distance:
- The azimuth is a real number between -180 ° and 180 °. It is 0 ° if the ofni is exactly north of the radar, 90 ° if the ofni is east.
- The distance is given in meters. We know that this data is not very precise (with a maximum deviation of 50 meters from the real value).

The objective of this exercise is to code an algorithm allowing to calculate the precise position of the ofnis in relation to the first buoy.

The entries are:
- the torques (azimuth, distance) obtained on the first buoy,
- the torques (azimuth, distance) obtained on the second buoy,
- the relative position of the second buoy with respect to the first.

All (x, y) coordinates are expressed in the NE convention, this means that the x axis points north and the y axis points east.

Simplifying assumptions:
- The ofnis are all perceived by the two radars (no ofnis by hiding another).
- The ofnis never got too close to each other. The distance between two ofnis is always greater than or equal to 250 meters.
- No ofnis are placed in line with the two buoys.

This code was written for a company project and is subjected to copyrights. I can discuss the project and the method in detail though but the code can't be made public. 
