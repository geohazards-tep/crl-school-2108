## Training - SNAP, Jupyter and the Geohazards Thematic Exploitation Platform 

#### Goal

The goal is to provide tools for the CRL School 2018 students to discover, access, process and analyse the results using Jupyter notebooks and thus providing means to repeat the approaches with other use cases and processing scenarios.


#### Training details

The training will use Jupyter notebooks and Python to exploit the Ellip and GEP platform APIs to: 

##### Lesson 1 - Coherence normalized difference for an earthquake with magnitude >5 

The goal of this Jupyter notebook is to:

Use the **py_earthquake** Python module to query USGS Earthquake Catalog via its API to retrieve the earthquake events over a certain area and time of interest with a configurable minimum magnitude. 

The **py_earthquake** Python module wraps the USGS Earthquake Catalog and provides a simple approach for discovering earthquakes using an area of interest, a time of interest and a minimum magnitude.

And then:

   * Discover Sentinel-1 SLC data for creating the coseismic and pre-seismic interferometric pairs
   * Use the Geohazards Thematic Exploitation Platform to generate the coseismic and pre-seismic interferograms with DIAPASON
   * Download the coherence products generated by DIAPASON on the Geohazards Thematic Exploitation Platform
   * Perform the coherence analysis
   * Plot the coherence normalized difference

##### Lesson 2 - Generate the coseismic interferogram with SNAP

First stage-in the coseismic interferometric pair discovered in the previous lesson.

Then use the SNAP Toolbox operators with Python to create a workflow that applies the SNAP Operators:

     - Orbit file correction
     - TOPSAR split
     - Back-Geocoding
     - Interferogram
     - TOPSAR Deburst
     - TOPSAR Merge
     - TopoPhaseRemoval
     - GoldsteinPhaseFiltering
     - Terrain correction

#### More information 

Check-out the discussions about this topic [here](http://discuss.terradue.com/c/geohazards/crl-school-2018)
