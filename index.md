## Screenshots

Middle of map with VIS disabled:
![Middle of map with VIS disabled](img/mid-no-vis.png)
Middle of map with VIS enabled:
![Middle of map with VIS enabled](img/mid-vis.png)

Note that various surfaces that should be visible are not rendered when VIS is enabled. These surfaces use displacement mapping, which is not yet supported in this project. Such surfaces require special handling in VIS, and these features of the Source Engine are not well documented.

Enclosed space with VIS disabled
![Enclosed space with VIS disabled](img/stairs-no-vis.png)
Enclosed space with VIS enabled
![Enclosed space with VIS enabled](img/stairs-vis.png)

Note the performance difference in an enclosed space. Without VIS culling, all faces in the map are rendered, bringing the FPS down to around 35. With VIS culling in a location without line-of-site to much of the map, far fewer faces are rendered, allowing the FPS to cap out at 60.
