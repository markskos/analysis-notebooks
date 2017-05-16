# ipython notebook examples of WiFi position analysis

There are three examples here,  CalculatePathDirections.ipynb,  Chi2_fit_Minuit.ipynb and LocationCombinations.ipynb .  
The first one takes in data of fitted positions of WiFi devices (smart phones) and plots
a flow diagram based on the calculated velocities from the positions in the data.  The second
notebook does a Chi2 minimization fit of actual measurements of WiFi signal strength picked
up by wireless routers to determine the positions of WiFi emitting devices. A minimum of 4 measurements
are needed to reconstruct the position.
The third notebook, LocationCombinations.ipynb, finds the stores that a WiFi device has visited.  The combinations of any
two stores visited are then determined.  The output is a dataframe that is based on a matrix where each element i,j contains the number
of devices that visited both stores i and j.   

## Calculating and plotting flow direction
### Requirements
For this notebook only the standard SciPy packages are needed: NumPy, Matplotlib, and Pandas.  All the 
data required for the notebook are in the data/ folder.

## Chi2 Fit
### Requirements
For this notebook one has to install the ROOT analysis package (from CERN).  It is free and can be downloaded 
from:  https://root.cern.ch/ .  The TMinuit library is used to do the minimization of the given Chi2 function.
The model for the propagation of the WiFi signals is given by the Friis equation in free space.# analysis-notebooks

## Location combinations
### Requirements
For this notebook the standard SciPy packages are needed: NumPy, Matplotlib, and Pandas, plus the mplPath library for determining if a point is inside a polygon.  All the 
data required for the notebook are in the data/ folder.
