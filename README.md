# Track Database

This is an attempt to represent all the BSCRA (and world's?) slot car tracks in a machine-readable representation, using json.

Ideally this should all be saved and maintained in a secure database, however we need to start somewhere.

The track-index.json is meant to be an index into the individual track files. This approach was chosen in preference to putting every track say into a single json file, in order to make the datasert more accessible and maintainable.

## Track Index

Should be self evident, it contains meta data that comprises: the searchable name of the track, a URL "pointer" where this index and the specific track files shall be found.

## Track File

