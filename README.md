# Restoring present-day crustal thickness using GPlates

This repository contains code that converts netCDF rasters to GPlates scalar coverages. The code runs on python and requires the following dependencies:
- pygplates
- numpy
- netCDF4

To connect a crustal thickness raster to a GPlates deforming mesh:
1. run the relevent cells in Crustal_thickness_restoration.ipynb.
2. Open the deforming plate model in GPlates and load in the new scalar_coverage.gpml file that you just created.
3. Click on the green reconstructed geometries layer for your new scalar coverage file and click "yes" beneath *Reconstruct using topologies* in the *Reconstruction Options* section. Under *Set Parameters*, make sure that the time span matches the time span of the deforming mesh.
4. Change the time slider in GPlates and see how the crustal thickness changes!
