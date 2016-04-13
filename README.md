# jsk_apc_2016_meshes

This repository contains the original of the mesh data in [jsk_apc](https://github.com/start-jsk/jsk_apc) for APC2016.  
`original` directory contains CAD files of the components made by Autodesk Inventor.  
`stl` directory contains STL files converted from Inventor Assemblies which consist of the components in `original` directory.

The mesh data in [jsk_apc](https://github.com/start-jsk/jsk_apc) for APC2016 were modified by MeshLab in order to reduce the polygon counts. The method of modifying is following:  

From the menu, select Filters > Remeshing, simplification and construction > Quadratic Edge Collapse Detection.   
Option Settings:
- Quality threshold: 1
- Preserve Boundary of the Mesh: Yes
- Boundary Preserving Weight: 1
- Preserve Normal: Yes
- Preserve Topology: Yes
- Optimal position of simplified vertices: Yes
- Planar simplification: Yes
- Weighted Simplification: No
- Post-simplification cleaning: Yes
- Simplify only selected faces: No  
