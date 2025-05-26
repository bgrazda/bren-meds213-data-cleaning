# Cleaning the shorebird survey data 


## The data set

ARCTIC SHOREBIRD DEMOGRAPHICS NETWORK [https://doi.org/10.18739/A2222R68W](https://doi.org/10.18739/A2222R68W)

Data set hosted by the [NSF Arctic Data Center](https://arcticdata.io) data repository 

Field data on shorebird ecology and environmental conditions were collected from 1993-2014 at 16 field sites in Alaska, Canada, and Russia.

![Shorebird, copyright NYT](https://static01.nyt.com/images/2017/09/10/nyregion/10NATURE1/10NATURE1-superJumbo.jpg?quality=75&auto=webp)


## DATA AND FILE OVERVIEW
The data folder, data/, contains two folders: raw/ and processed/. The structure of the data folder is as follows:

data
├── processed
│   ├── all_cover_fixed_LIZPETERSON.csv
│   ├── snow_cover.csv
│   └── species_presence.csv
├── raw
│   ├── 01_ASDN_Readme.txt
│   ├── ASDN_Daily_species.csv
└── └── ASDN_Snow_survey

- `all_cover_fixed_LIZPETERSON.csv`: Cleaned snow survey data
- `snow_cover.csv`: Partially cleaned snow cover survey data (only the snow_cover column was cleaned)
- `species_presence.csv`: Cleaned species data
- `01_ASDN_Readme.txt`: Original metadata from ASDN
- `ASDN_Daily_species.csv`: Species survey data from ASDN
- `ASDN_Snow_survey`: Snow cover survey data from ASDN


**Additional RelatedDatasets from Artic Data Center (not included)**
- ASDN_Daily_species_effort.csv
- ASDN_Geodata.csv
- ASDN_Invert_biomass.csv
- ASDN_Lemming_counts.csv
- ASDN_Lemming_nests.csv
- ASDN_Lemming_trap.csv
- ASDN_Pred_nests.csv
- ASDN_Pred_point_counts.csv
- ASDN_Bird_resights.csv
- ASDN_Bird_sexes.csv
- ASDN_Camp_info.csv
- ASDN_Camp_staff.csv
- ASDN_Daily_pred_lemm.csv
- ASDN_Daily_species.csv
- ASDNDaily_species_effort.csv

The version of this dataset was created for EDS 213: Databases and Data Management at the Bren School of Environmental Science & Management. The original version of this dataset can be found at the [Arctic Shorebord Demographics Network](https://arcticdata.io/catalog/view/doi:10.18739/A2222R68W).




  






Data were not collected every year at all sites. Studies of the population ecology of these birds included nest-monitoring to determine the timing of reproduction and reproductive success; live capture of birds to collect blood samples, feathers, and fecal samples for investigations of population structure and pathogens; banding of birds to determine annual survival rates; resighting of color-banded birds to determine space use and site fidelity; and use of light-sensitive geolocators to investigate migratory movements. 

Data on climatic conditions, prey abundance, and predators were also collected. Environmental data included weather stations that recorded daily climatic conditions, surveys of seasonal snowmelt, weekly sampling of terrestrial and aquatic invertebrates that are prey of shorebirds, live trapping of small mammals (alternate prey for shorebird predators), and daily counts of potential predators (jaegers, falcons, foxes). Detailed field methods for each year are available in the `ASDN_protocol_201X.pdf` files. All research was conducted under permits from relevant federal, state, and university authorities.


See `01_ASDN_Readme.txt` provided in the [course data repository](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-spring-2024-class-data) for full metadata information about this data set.

