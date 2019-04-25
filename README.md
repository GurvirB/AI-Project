# Predictive Aircraft Maintenance
## Introduction:
This project has been done in fulfillment to the CS595a - Artificial Intelligence course requirement. The aim of the project is to predictive the remaining useful life (RUL) of an engine at any instance of its lifetime using the concepts of neural networks in Artificial Intelligence.

## Problem:
Every year the aviation industry incurs huge direct (i.e. plane loss,after damage repair,life and personal loss, legal costs) and indirect costs (i.e. customer disatisfaction, reputation damage) due to a failure in any of the equipments currently deployed over the aircraft. Therefore, it is to the interest of the aviation companies to look for a solution how they can predict the time when any of the mechanical parts would need a maintenace.
which leads to the concept of predictive maintenance.Predictive maintenace determines the condition of an in-use equipment of the aircraft and predict when it would require the maintenance.
The hundreds of the sensors used in the airplanes produce sufficiently large amounts of data, which can be read and analyzed to see and predict when an engine can be expected to fail or atleast when it would need a maintenace. The same approach has been used for the completion of this project.

## Data:
The data for this project has been taken from NASA's Turbofan Engine Degradation Simulation, wherein they used the simulated run to failure events from 100 different engines. The data package comes with 4 datasets each for training and testing the model and one set containing RUL values.
### Training datasets: 
To prepare this dataset, all the 100 engines were run to failure.
### Testing datasets:
For these datasets, the engines were stopped randomly during their operational times.
### RUL datasets:
These datasets contain the values of the cycles for which the engines in the testset could have run more. Hence, adding the maximum number of cycles for the engines in he test set to the RUL given in the RUL dataset, will give the actual RUL for any engine.
