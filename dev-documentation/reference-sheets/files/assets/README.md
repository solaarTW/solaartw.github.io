# ▫ Assets

## What is an asset? <a href="#what-is-an-asset" id="what-is-an-asset"></a>

An asset is a specific, objectified concept in the game that can be highly detailed like a blade of grass, or larger like a building, or intangible like sound effects. Unity defines an asset as, "Shorthand for anything that goes into a video game – characters, objects, sound effects, maps, environments, etc." Every asset is defined in a set of [normalized](https://en.wikipedia.org/wiki/Database\_normalization) asset files that describe its relationship to the game, other assets, and itself.

## Visual Asset-Related File Formats <a href="#visual-asset-related-file-formats" id="visual-asset-related-file-formats"></a>

The following list contains file formats that are used to compose visual assets such as vehicles and weapons.The community-devloped tool **WolvenKit** can be used to browse game archives and extract game files. [Learn more](https://wiki.redmodding.org/wolvenkit/)​

| File                               | Description                                                                         |
| ---------------------------------- | ----------------------------------------------------------------------------------- |
| MESH                               | 3D models                                                                           |
| XBM                                | 2D textures                                                                         |
| ENT (entity)                       | Parent file for most visual assets which is directly linked by the Tweak DB         |
| APP (appearance)                   | Sets up appearances for assets such as NPCs and vehicles referenced by entity files |
| MT (material template)             | Base shader files for REDengine                                                     |
| MI (material instance)             | Instanced shaders for mesh materials                                                |
| MLMASK (multilayered mask)         | Mask component of the Multilayer supershader                                        |
| MLSETUP (multilayered setup)       | Material setup component of the Multilayer supershader                              |
| MLTEMPLATE (multilayered template) | Pre-defined tiling surface component of the Multilayer supershader​                 |
| HP (hair profile)                  | Color ramp data to set colors for meshes using the hair shader​                     |

## Visual Asset Graphs <a href="#visual-asset-graphs" id="visual-asset-graphs"></a>

![](https://820263885-files.gitbook.io/\~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2F4gzcGtLrr90pVjAWVdTc%2Fuploads%2FtGNbHSWif0FdRmUZrTYK%2FCP2077%20Vehicle%20Example.svg?alt=media\&token=0e9997cf-6ac3-461a-b00d-e590615a2616)​
