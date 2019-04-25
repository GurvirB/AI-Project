# Predictive Aircraft Maintenance
## Instructions to download the project:
1. Click on Clone or download option in green at the top right corner of the repository.
2. Download as zip.
3. Select open or save as option depending on how you want to access.
4. Extract the files from the downloaded zip folder.
5. Open the jupyter notebook from anaconda (you may need to install anaconda if not already present) and click on top right icon to upload the notebook.
6. To choose the files, scroll to the .ipnyb file in the extracted folder of step 4.
7. Once the upload is complete, run the jupyter notebook.

## Software requirements to run the uploaded jupyter notebook:
1. Python 3.6
2. Keras 2.1.1
3. TensorFlow 1.3.0
4. numpy 1.13.3
5. matplotlib 2.0.2
6. scikit-learn 0.19.0
7.pandas 0.20.3

If the jupyter notebook does not recognize any of the above libraries, you can install the libraries from the notebook's terminal.
PLease refer the below link if you face any difficulty while installing the same: 
https://jakevdp.github.io/blog/2017/12/05/installing-python-packages-from-jupyter/ 
If you don't have anaconda installed on your computer, you can use the below link to install it:
https://www.anaconda.com/distribution/

## Introduction:
This project has been done in fulfillment to the CS595a - Artificial Intelligence course requirement. The aim of the project is to predictive the remaining useful life (RUL) of an engine at any instance of its lifetime using the concepts of neural networks in Artificial Intelligence.

## Problem:
Every year the aviation industry incurs huge direct (i.e. plane loss,after damage repair,life and personal loss, legal costs) and indirect costs (i.e. customer disatisfaction, reputation damage) due to a failure in any of the equipments currently deployed over the aircraft. Therefore, it is to the interest of the aviation companies to look for a solution how they can predict the time when any of the mechanical parts would need a maintenace.
which leads to the concept of predictive maintenance.Predictive maintenace determines the condition of an in-use equipment of the aircraft and predict when it would require the maintenance.
The hundreds of the sensors used in the airplanes produce sufficiently large amounts of data, which can be read and analyzed to see and predict when an engine can be expected to fail or atleast when it would need a maintenace. The same approach has been used for the completion of this project.

## Data:
The data for this project has been taken from NASA's Turbofan Engine Degradation Simulation, wherein they used the simulated run to failure events from 100 different engines. The data package comes with 4 datasets each for training and testing the model and one set containing RUL values.
Datasets are available at: https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/ .
Datasets have also been uploaded in the repository's CMAPSSData folder.
### Training datasets
To prepare this dataset, all the 100 engines were run to failure.
### Testing datasets
For these datasets, the engines were stopped randomly during their operational times.
### RUL datasets
These datasets contain the values of the cycles for which the engines in the testset could have run more. Hence, adding the maximum number of cycles for the engines in he test set to the RUL given in the RUL dataset, will give the actual RUL for any engine.

## Approach:
This project uses the regression approach of the machine learning to predict the RUL for an engine. Keras sequenatila model has been used with SGD at the learning rate = 0.001 to train the system.
Training data was split and allocated 10% of it for the system validation. MAE and accuracy are used as metrics.
History has been plotted to show how the system performs during training. Also, a graph and a pandas dataframe have been plotted to compare the real RUL to the predicted RUL.


