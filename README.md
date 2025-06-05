# bifrost-openswarm-modules
Developed modules for BIFROST within the Openswarm project.
Please refer to the single repositories for more information and documentation. Here just a list of the developed modules with links to their repositories is provided here:

## Asset-Simulator
This module simulates all assets of the Energy Community (EC) tackled in the PoC1 use cases of the OpenSwarm project.

Repository: https://github.com/openswarm-eu/bifrost-openswarm-module-asset-simulator

This module Reads in data from `./data/csv/profile-data.csv` and adds the PV or electro vehicle (EV) data to the buildings depending on their stackable for the `POWERGRID-CONNECTOR`. It also provides measurement data and limits for feeder line grid sensors.
  - PV data requires `SOLAR-PANEL`
  - EV data `CHARGING-POLE`
  - Grid Sensor Measurements requires `GRID-SENSOR`
