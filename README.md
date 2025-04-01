# MASTER
## Multiple ASpect TrajEctoRy management and analysis

------------------------------------------------------
In order to monitor the tourism flow in Santorini Island, the questions we want to answer are:

**a)** Which is the origin Country of travelers? 

**b)** How long do the tourists stay in Santorini? 

**c)** Are the first-time visitors and returning visitors behaving differently?

**d)** Can we predict the tourist arrival flows? 

**e)** Which is the qualitative level of satisfaction / dissatisfaction of the user?

The project is organized as follow:

```
MASTER/
│
├── datasets/
│   ├── airbnb/
│   ├── flights/
│   ├── tweets/
│   └── osm/
│
└── research_questions/
    │
    ├── RQ_A_which_is_the_origin_country_of_travelers/
    │   ├── outputs/
    │   └── code.ipynb
    │
    ├── RQ_B_how_long_do_tourist_stay/
    │   ├── outputs/
    │   └── code.ipynb
    │
    ├── RQ_C_are_the_first_visitors_and_returning_visitors_behaving_differently/
    │   ├── outputs/
    │   └── code.ipynb
    │
    ├── RQ_D_predict_arrival_departure_flow/
    │   ├── outputs/
    │   └── code.ipynb
    │
    └── RQ_E_which_is_the_qualitative_level_of_satisfaction_dissatisfaction_of_users/
        ├── outputs/
        └── code.ipynb


```

In the ```dataset``` folder there is one subfolder for each dataset needed for the analysis. 

In the ```twitter``` folder, you can directly insert files from the Twitter streaming API. 

In the ```airbnb``` folder, you can insert a ```airbnb.csv``` file with at least the following columns:
    
- ```id```: the room/flat identifier;
- ```name```: the room/flat name;
- ```neighbourhood```: the location name;
- ```latitute```: the room/flat latitude;
- ```longitude```: the room/flat longitude;
- ```mimimum_nights```: the minimum number of nights required to book.

In the ```osm``` folder, you can insert the ```santorini.gpx``` file containing the trajectories from OpenStreetMap API (you can download it from JOSM application - https://josm.openstreetmap.de/, selecting the bounding box of Santorini).

In the ```flights``` folder, you can insert files containing the information about the number of domestic and international passengers per month and year.

In the ```research_questions``` folder, you can find a folder for each of the five questions described above. In each of these folders, you find a file with the ```.ipynb``` extension in which we analyse the datasets described above and an ```output``` subfolder with the results (represented with both plots and description files).

## Installation

If you want to run code locally, you can download the entire repository and install the requirements as follow:

    pip install -r requirements.txt

## DOI
[![DOI](https://zenodo.org/badge/599025662.svg)](https://doi.org/10.5281/zenodo.15120715)
