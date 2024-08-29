# Maps
The game's five islands are organized in maps. The game's maps are in the BIN format and are found in `doshin/maps/` (PAL) or
`Doshin/maps/` (JP).
# The Map Format
The game's maps are in the BIN file format. It is a binary file format which contains it's respective map's geometry and GEN data.

The format consists of three segments: `HMAP`, `IDEF` and `IMAP`. 
* `HMAP` is mainly unknown in what it contains. It most likely contains the map geometry, but it is theorized that it might contain
matrix data.
* `IDEF` is GEN-related and seems to contain object definiton data and object collision and scaling.
* `IMAP` seems to contain the actual GEN data of maps (e.g. position and rotation of objects).

# Editing Maps
Currently, there is no known way of editing maps. Hex edits have been tried, but they don't appear to have worked and the map
format has not been cracked.

VicsGithub (the owner of this repository) is currently working on a tool for editing maps called "Kyojin Studio".
