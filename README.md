# Challenge "Help Paris become a Smart City"

[This project is part of the AI Engineer cursus on OpenClassrooms]

We are provided with a dataset from [opendata.paris](https://opendata.paris.fr/explore/dataset/les-arbres) which lists 200 137 trees belonging to the city of Paris.

There are 18 columns used to describe each tree:
- *id*: the tree's id in the dataset
- *type_emplacement*: the area's type (trees, flowers, ....)
- *domanialite*: the domain type (parcs, cimeterry, some administration...)
- *arrondissement*: the Paris' district (25 in total)
- *complement_addresse*: some address informations
- *numero*: the street number
- *lieu*: the address
- *id_emplacement*: the area's id
- *libelle_francais*: the commun french name
- *genre*: the type
- *espece*: the species
- *variete*: the variety 
- *circonference_cm*: the circumference in centimeters
- *hauteur_m*: the height in meters
- *stade_developpement*: the developement stage (Young, Young Adult, Adult, Mature)
- *remarquable*: indicates if the tree has something special
- *geo_point_2d_a*: the latitude
- *geo_point_2d_b*: the longitude

> The goal is to analyse this dataset in order to find some interesting ways to optimize the rounds for the maintenance of the city's trees.

## Running the notebook online

This notebook is quite heavy and it may not correctly display on Github.
However it can be displayed at the following address: [https://nbviewer.org/github/Valkea/OC_AI_02/blob/main/EDA.ipynb](https://nbviewer.org/github/Valkea/OC_AI_02/blob/main/EDA.ipynb)

**It will takes some time to load because of the several folium maps**, so be sure to give it the time to correctly initialize.

## Running the notebook locally

In order to use this project locally, you will need to have Python and Jupyter notebook installed.
Once done, we can set the environment by using the following commands:

### First, 
let's duplicate the project github repository

```bash
>>> git clone https://github.com/Valkea/OC_AI_02 
>>> cd OC_AI_02
```

### Secondly,
let's create a virtual environment and install the required Python libraries

(Linux or Mac)
```bash
>>> python3 -m venv venv
>>> source venv/bin/activate
>>> pip install -r requirements.txt
```

(Windows):
```bash
>>> py -m venv venv
>>> .\venv\Scripts\activate
>>> py -m pip install -r requirements.txt
```

### Thirdly,
let's configure the virtual environment for Jypiter notebook


#### Install jupyter kernel for the virtual environment using the following command:

```bash
>>> ipython kernel install --user --name=venv
```

#### Run the jupyter notebook

```bash
>>> jupyter notebook notebook.ipynb
```

#### Select the installed kernel
Click on the kernel and click change kernel you will be able to see the kernel you just created.
![alt text](medias/venv_selection.png)

## Uninstalling the venv kernel
Once done with the project, the kernel can be removed using the following command:

```bash
jupyter-kernelspec uninstall venv
```

