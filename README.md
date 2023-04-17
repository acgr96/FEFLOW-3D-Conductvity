# FEFLOW-3D-Data
Script that can couple information from 3D point cloud models to a mesh exported from FEFLOW, then convert result to a FEFLOW readable table for parameter 
linkage.

With this script, one can generate custom point clouds of data that can be read directly into DHI FEFLOW for parameterization. The script is written for 
hydraulic conductivity (Kx) but can be easily altered for other parameters. It was written with the express purpose of converting large 3D model of RQD exported 
from Leapfrog, converting the RQD values to conductivity through a defined function, and exporting the result back to a FEFLOW readable xlsx table. AS such,
it demosntrateds a few other tools that may be useful outside of this script such as:
- Applying custom mathematical function to pandas dataframe
- Inner merge of data frames, and general operations on high-memory datasets, using Dask in tandem with pandas
- Indexing and merging large data sets with "near equal" data by normalizing key data to integers and building a summation index.

Repository contains separate (work in progress) script for 3D visualization of data being manipulated. This will eventually be integrated into the main notebook.
