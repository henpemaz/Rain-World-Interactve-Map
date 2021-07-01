# Rain-World-Interactive-Map
A Rain World interactive map using leaflet and GeoJSON data exported from the game files.

[(Link to the map page)](https://henpemaz.github.io/Rain-World-Interactive-Map/index.html)

This project consists of two parts
- Some python code for reading through the game files and exporting anything of interest as geojson features using the dev-map coordinates, also creates the low-res room tiles to be used by the map from the merged-screenshots collection by AndrewFM.
- The front-end app in plain html css and javascript using Leaflet for the map, all static files so it can be hosted in github.

The current state of this project is: a mess. The python script is barely readable at this point and I'm a terrible front-end developer.

The currently tracked objects from the game are:
- room cameras (they define how to place the screenshots in the map)
- room names
- room connections
- room.txt-defined throwables (apparently broken oops)
- spawns and lineages (including offscreen), filtered by difficulty

The immediate to-do list for this project is:
- place icons for the most common room tags like "shelter", "scavoutpost" and "swarmroom"
- shelters filterable by difficulty
- in-room shortcuts
- karma for gates
- read and add placed-objects
    - popcorn, fruit, placed spears
    - soundtrack triggers!!!
    - pealrs and echos 
- offscreen transportation pipes (scav-pipes)
- rework map graphics, switch from image overlays to tile-sets
    - kind of a big deal, would require some python-pillow wizardry to stitch up the whole map and chop it down at the different zoom levels, there's probably tools for that around.
- make things pretty 🥺

It should be possible to generate a similar map for a modded install of the game with hopefully little rewriting of the code. I might do that in the future, or maybe you could try it now.

If you wish to contribute, hmu on Discord
