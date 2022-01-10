# Hypertention
* * *
A case study about the effect of hypertention in society

## Description
* * *
This repository contains the code for the final assignemtn for programming 1, which shows the result of a study about hypertention in the the world and the Netherlands

### Data
The original plan was to create a sort of 'olfactometer' to test the attraction of humans to mosquitoes. The olfactometer contained a box, where the mosquitoes were led loose, and a cylinder which split into two directions, so it was y-shaped. At both ends of these two cylinders a hand could be inserted to test several variables(i.e. lavender oil, cinnamon oil, etc.). The mosquitoes were counted when all of them were at the end of either one of the cylincers. Then, the two cylinders were compared and a conclusion could be drawn. 

However, the experiments were not actualized because the mosquitoes had died and new mosquitoes could not be aquired in the short timeframe that was left. The solution to this problem was to generate mock data. In order to generate data a model was build which could create a probability that a mosquito would choose to go to the right chamber instead of the left chamber. This model contained several variables, including: if a substance was applied or not, blood type, weight, body temperature and blood glucose level of the individuals that were in the left and right chamber. Assumptions were made about the importance of each variable which was drawn from current literature. 

**Formula**:  

![equation_f](http://www.sciweavers.org/download/Tex2Img_1641568101.jpg)  

![equation_p](http://www.sciweavers.org/download/Tex2Img_1641568268.jpg)

This probability(p) was then used to create a number, using a binomial distribution, which represents the amount of mosquitoes that went to the right chamber.

### Data description

The different columns of the table are described in the documentation directory [here](/documentation/data_table_documentation.md)

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
How to run the code?


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


## Acknowledgements
* * *
We want to thank two people in particular. First, we want to thank René van Koldam because he helped us tremendously with creating the experimental setup. Second, we want to thank ir. PFA (Pieter) Rouweler for providing us with a batch of mosquito larvae. 


## License
* * * 
This project contains a MIT [license](./LICENSE.md)


## References
* * *

* ***[1]***: The pandas development team, **pandas-dev/pandas: Pandas**, feb, 2020, Zenodo, latest, [10.5281/zenodo.3509134](https://doi.org/10.5281/zenodo.3509134)
* ***[2]***: Bokeh Development Team, **Bokeh: Python library for interactive visualization**, 2018, [https://bokeh.pydata.org/en/latest/](https://bokeh.pydata.org/en/latest/)
* ***[3]***: HoloViz, **Panel: A high level app and dashboarding solution for Python**, 24, 8, 2018, panel.holoviz.org, 0.12.1, [http://panel.holoviz.org](http://panel.holoviz.org) 

