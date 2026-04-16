# bifrost-openswarm-modules
Developed modules for BIFROST within the Openswarm project.
Please refer to the single repositories for more information and documentation. Here just a list of the developed modules with links to their repositories is provided here:

## Content

- [Asset-Simulator](#asset-simulator)
- [Community-Controller](#community-controller)
- [Controller-Connector](#controller-connector)
- [Community-Controller Nadzuro2](#community-controller-nadzuro2)


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

## Community-Controller Nadzuro2
This repository contains the files to create the SCT-supervisors for the [Community-Controller](#community-controller)

Repository: 
  - https://code.siemens.com/openswarm/energy-community-controller-nadzoru2
  - https://github.com/openswarm-eu/bifrost-openswarm-module-controller-nadzoru2

# Acknowledgement

Part of the source code in this repository is developed within the frame and for the purpose of the OpenSwarm project. This project has received funding from the European Unioan's Horizon Europe Framework Programme under Grant Agreement No. 101093046.

![OpenSwarm - Funded by the European Union](logos/ack.png)
