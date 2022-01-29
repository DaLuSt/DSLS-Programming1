# Prevalance of hypertention from a sample population as compaired to the Netherlands
* * *
A case study about the effect of hypertention in society Daan Steur

## Description
* * *
This repository contains the code for the final assignemtn for programming 1, which shows the result of a study about hypertention in the the world and the Netherlands

### Data
High blood pressure (hypertension) is a common condition in which the long-term force of the blood against your artery walls is high enough that it may eventually cause health problems, such as heart disease. But what parameters influence the occurrence of hypertension. can the area of residence or smoking habits be of influence. How does the Netherlands compare to worldwide hypertension percentages. 


### Data description


Stroke prediction data:
1) id: unique identifier
2) gender: "Male", "Female" or "Other"
3) age: age of the patient
4) hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6) ever_married: "No" or "Yes"
7) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8) Residence_type: "Rural" or "Urban"
9) avg_glucose_level: average glucose level in blood
10) bmi: body mass index
11) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"*
12) stroke: 1 if the patient had a stroke or 0 if not
*Note: "Unknown" in smoking_status means that the information is unavailable for this patient

Source: https://www.kaggle.com/fedesoriano/stroke-prediction-datasetpres

Blood pressure: evolution of blood pressure over time (1975-2015 yearly):
1) Country/Region/World
2) ISO
3) Sex
4) Year
5) Mean systolic blood pressure (mmHg)
6) Mean systolic blood pressure lower 95% uncertainty interval (mmHg)
7) Mean systolic blood pressure upper 95% uncertainty interval (mmHg)
8) Mean diastolic blood pressure (mmHg)
9) Mean diastolic blood pressure lower 95% uncertainty interval (mmHg)
10) Mean diastolic blood pressure upper 95% uncertainty interval (mmHg)
11) Prevalence of raised blood pressure
12) Prevalence of raised blood pressure lower 95% uncertainty interval
13) Prevalence of raised blood pressure upper 95% uncertainty interval

Source -Country specific data for all counties and global data-: https://ncdrisc.org/data-downloads-blood-pressure.html

Hypertension per age and sex per 1000 people in the Netherlands 2020:
1) Age
2) Man
3) Vrouw
4) Totaal

Source: https://www.volksgezondheidenzorg.info/onderwerp/bloeddruk/cijfers-context/huidige-situatie#:~:text=Ongeveer%202%2C8%20miljoen%20Nederlanders,gedurende%20een%20bepaald%20jaar. (Government reference data)


## Installation
* * *

### Single install
The easiest way to install all the required packages is via conda. How to install conda on your system can be found [here](https://docs.anaconda.com/anaconda/install/index.html).

To create a new environment which contains all the required packages plus the right version run the following code:

```bash
  conda env create -f environment.yml
```

This will create a new environment named `mosquito_env` which can be used to run this repository.

> NOTE: the environment.yml is located in the install/ directory [here](install/environment.yml).

### Multiple installs
An other option is to install each package seperately, either with conda or pip.

conda:
```bash
  conda install <PACKAGE>=<VERSION>
```

pip
```bash
  pip install <PACKAGE>==<VERSION>
```

> NOTE: make sure to use the correct versions, which are listed [here](#packages).

## Getting started
* * *
To see the results run the Prog1_Final_Assignment.ipynbnotebook from top to bottom.

Open the jupyter notebook
run all code


## Requirements
* * *
| Software                          | Version  |
| --------------------------------- | :------: |
| [Python](https://www.python.org/) | `3.9.7`  |    


## Packages
* * *
| Package                                | Version  |
| ---------------------------------------| :------: |
| [numpy](https://numpy.org/)            | `1.21.2` |
| [pandas](https://pandas.pydata.org/)   | `1.3.3`  |
| [bokeh](https://bokeh.org/)            | `2.3.3`  |
| [panel](https://panel.holoviz.org/)    | `0.12.1` |
| [holoviews](https://holoviews.org/)    | `1.14.6` |
| [hvplot](https://hvplot.holoviz.org/)  | `0.7.3`  |
| [scipy](https://scipy.org/)            | `1.7.1`  |
| [jupyter](https://jupyter.org/)        | `1.0.0`  |
| [Panel](http://https://panel.org/)     |`0.12.6`  |


## Acknowledgements
* * *



## License
* * * 
This project contains a MIT [license](./LICENSE.md)


## References
* * *

* ***[1]***: The pandas development team, **pandas-dev/pandas: Pandas**, feb, 2020, Zenodo, latest, [10.5281/zenodo.3509134](https://doi.org/10.5281/zenodo.3509134)
* ***[2]***: Bokeh Development Team, **Bokeh: Python library for interactive visualization**, 2018, [https://bokeh.pydata.org/en/latest/](https://bokeh.pydata.org/en/latest/)
* ***[3]***: HoloViz, **Panel: A high level app and dashboarding solution for Python**, 24, 8, 2018, panel.holoviz.org, 0.12.1, [http://panel.holoviz.org]
*(http://panel.holoviz.org) 

