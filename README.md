# the-threat-of-aggregated-cyberattacks-on-power-grids
This repository contains instructions and configuration files for the Master's thesis "The Threat of Aggregated Cyberattacks on Power Grids"

# Power Grid Simulator 
Link to PowerWorld: https://www.powerworld.com/. 

PowerWorld Demo: https://www.powerworld.com/download-purchase/demo-software

# Power Grid Model
The power grid model WSCC 9-bus system can be found at https://electricgrids.engr.tamu.edu/electric-grid-test-cases/. Configuration to the model is described in Chapter 4, which involves adding a governor to the slack generator.

# Implemented Attack Strategies 
Some of the evaluated attack strategies are found in the file "pw_transient_stability_analysis_config.aux".

# Setup

Pre-requisites:
1. Download PowerWorld
2. Download WSCC 9-bus system
3. Launch the WSCC 9-bus system by executing the PowerWorld binary

Generator configurations
4. Right-click the generator called "slack" on Bus1 in the one-diagram, and select "Generator Information Dialog for Bus1 (1)#1"
5. Navigate to the Stability tab and thereafter the sub-tab Governors
6. Select Insert and then locate the IEEEG2 governor model, click OK and then OK on the "Generator Information Dialog for Bus1 (1)#1"

Launch the transient stability simulator:
7. The Transient Stability simulator can be found under the tab "Add Ons" in the top-banner
8. Click "Load All Settings From" and select the downloaded pw_transient_stability_analysis_config.aux"
9. Simulations are started from the Simulation tab. Select the simulation to be executed and press "Run Transient Stability".
10. Graphs can be configured from the Plots tab
