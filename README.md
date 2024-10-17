# Autonomous Navigation of Lightweight UAVs in GPS-denied environments
Final Bachelor Thesis | Iago Senén Fernández García |  Aerospace Engineering UC3M

Grade: 10/10, nominated to honours (MH)

## Structure of this repo
This repository is structured as follows:

* **Data Adquisition**: contains raw flight logs and images obtained from testing aircraft.
* **Data Cleaning**: contains chopped and pre-processed flight logs for each of the performed flights
* **Data Analysis** : contains the python notebooks used to extract useful metrics and information from the data
* **Manufacturing**: contains all the 3D files and laser cutting boards in order to manufacture the aerial platform "RoadRunner" for testing different visual-based navigation solutions. 
> ⚠️ To Be Completed, some missing files. I want to upload them so that they are ready to cut/print. ⚠️
* The Original PDF submitted for grading. 

## How to use this repo
In order to start working with this repository start by downloading miniconda [here](https://docs.anaconda.com/miniconda/) and use the given environment.yaml file to recreate the conda environment. You can later execute the jupyter notebooks to recreate results.

```
conda env create --file environment.yaml
```

Followed by the activation of the given environment:
```
conda activate tfg-gps-denied-navigation
```
And enabling the new Python kernel based on the installed environment:
```
python -m ipykernel install --user --name tfg-gps-denied-navigation --display-name "tfg-gps-denied-navigation"
```

Note: Use the command "python3" for Mac users.


