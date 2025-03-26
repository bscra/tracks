# Track Database

This is an attempt to represent all the BSCRA (and world's?) slot car tracks in a machine-readable representation, using json.

Ideally this should all be saved and maintained in a secure database, however we need to start somewhere.

The track-index.json is meant to be an index into the individual track files. This approach was chosen in preference to putting every track say into a single json file, in order to make the datasert more accessible and maintainable.

## Track Index

Should be self evident, it contains meta data that comprises: the searchable name of the track, a URL "pointer" where this index and the specific track files shall be found.

## Track File

This contains some basic identifying information about the track and detailed information about each of the lanes. 

The lanes shall be described by a series of x, y points and vectors. The x direction is assumed to be the cars' direction of travel, the conventional positive y direction points to the left and the negative direction to the right.

Tracks are generally split and marked into segments that are ~1/100 of the lane length. For example Castle is nominally a 100' lap length so the segments are 12". In reality they are more like 11.5" and becuase the track was made in the "good olde days" with a hand router it's not precise.

So the red lane main straight at Castle could be represented by say a starting reference point of 0,0, the first segment marker at 11.5,0 etc. If the track could be mapped there would be 99 points per lane - one for each segment.

For a more detailed representation of the track, each lane could be represented more finely by collecting points every centimeter say. These could them be chained together to build a vector, graphic representation of each lane.
