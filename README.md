# jsk_apc_2016_meshes

This repository contains the original of the mesh data in [jsk_apc](https://github.com/start-jsk/jsk_apc) for APC2016.
`original` directory contains CAD files of the components made by Autodesk Inventor.
`stl` directory contains STL files converted from Inventor Assemblies which consist of the components in `original` directory.

The mesh data in [jsk_apc](https://github.com/start-jsk/jsk_apc) for APC2016 were modified from STL data in `stl/visual` and `stl/collision` by MeshLab in order to reduce the polygon counts. The method of modifying is following:

From the menu, select Filters > Remeshing, Simplification and Reconstruction > Quadric Edge Collapse Decimation.
Option Settings:
- Percentage reduction (0..1): 0.3
- Quality threshold: 0.3
- Preserve Boundary of the Mesh: No
- Boundary Preserving Weight: 1
- Preserve Normal: No
- Preserve Topology: No
- Optimal position of simplified vertices: Yes
- Planar simplification: No
- Weighted Simplification: No
- Post-simplification cleaning: Yes
- Simplify only selected faces: No

I printed STL models in `stl/output_to_printer` by 3D printers to make grippers.
