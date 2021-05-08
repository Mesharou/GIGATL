# GIGATL


![image info](./Figures/gigatl1_1h_tides_surf_vrt38160_dpi100.png)

GIGATL is a set of Atlantic Ocean numerical simulations performed with the Coastal and Regional Ocean COmmunity model ([CROCO](https://www.croco-ocean.org/)), which is built upon the Regional Oceanic Modeling System (ROMS).

The simulation domain covers the Atlantic Ocean. Simulations are available in several resolutions:

 - **GIGATL1** =  < 1 km in the horizontal with 100 "topography-following" vertical levels
 - **GIGATL3** = 3 km in the horizontal with 100 "topography-following" vertical levels
 - **GIGATL6** = 6 km in the horizontal with 50 "topography-following" vertical levels
 - **GIGATL24** = 24 km in the horizontal with 50 "topography-following" vertical levels

--

### Configuration

The GIGATL24, GIGATL6, and GIGATL3 simulations are initialized in January 2004. The initial and boundary conditions are supplied by the Simple Ocean Data Assimilation (SODA). 

The GIGATL1 simulations are initialized in July 2007 using outputs from the GIGATL3 simulations. The boundary conditions are supplied by SODA. 

All simulations are forced by hourly atmospheric forcings from the Climate Forecast System Reanalysis (CFSR) using a bulk formulation with relative winds.

Each simulation has been run in two versions including tides or not. Simulations with tides include barotropic tidal forcing at the boundaries and tidal potential and self attraction that are taken respectively from TPXO7.2 and GOT99.2b. 

The bathymetry is taken from the SRTM30plus dataset. 

The k-epsilon turbulence closure scheme is used to parameterize vertical mixing, and the Canuto A stability function formulation is applied. There is no explicit lateral diffusivity in the simulation. 

The effect of bottom friction is parameterized through a logarithmic law of the wall with a roughness length $Z_0 = 0.01$ m. 


--









[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by-nc-sa/4.0/)
