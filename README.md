# bifrost-openswarm-modules
Developed modules for BIFROST within the Openswarm project.
Please refer to the single repositories for more information and documentation. Here just a list of the developed modules with links to their repositories is provided here:

## Content

- [Asset-Simulator](#asset-simulator)
- [Community-Controller](#community-controller)
- [Controller-Connector](#controller-connector)


## Asset-Simulator
This module simulates all assets of the Energy Community (EC) tackled in the PoC1 use cases of the OpenSwarm project.

Repository: 
  - https://code.siemens.com/openswarm/energy-community-asset-simulator
  - https://github.com/openswarm-eu/bifrost-openswarm-module-asset-simulator

This module Reads in data from `./data/csv/profile-data.csv` and adds the PV or electro vehicle (EV) data to the buildings depending on their stackable for the `POWERGRID-CONNECTOR`. It also provides measurement data and limits for feeder line grid sensors.
  - PV data requires `SOLAR-PANEL`
  - EV data `CHARGING-POLE`
  - Grid Sensor Measurements requires `GRID-SENSOR`


## Community-Controller

OpenSwarm community controller based on the [Data Distribution Agent (DDA)](https://github.com/openswarm-eu/dda).

Repository:
  - https://code.siemens.com/openswarm/energy-community-controller
  - https://github.com/openswarm-eu/bifrost-openswarm-module-controller

## Controller-Connector
This BIFROST module connects the [OpenSwarm energy community controller](#community-controller) to the BIFROST virtual testbed.

Ensure, that you either have the openswarm energy community controller docker images
* cr.siemens.com/openswarm/energy-community-controller/charger 
* cr.siemens.com/openswarm/energy-community-controller/pv
stored locally or access to the docker repo.

Repository: 
  - https://code.siemens.com/openswarm/energy-community-controller-bifrost-connector
  - https://github.com/openswarm-eu/bifrost-openswarm-module-controller-connector
