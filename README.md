# Cleaning the shorebird survey data 


## The data set

ARCTIC SHOREBIRD DEMOGRAPHICS NETWORK [https://doi.org/10.18739/A2222R68W](https://doi.org/10.18739/A2222R68W)

Data set hosted by the [NSF Arctic Data Center](https://arcticdata.io) data repository 

Field data on shorebird ecology and environmental conditions were collected from 1993-2014 at 16 field sites in Alaska, Canada, and Russia.

![Shorebird, copyright NYT](https://static01.nyt.com/images/2017/09/10/nyregion/10NATURE1/10NATURE1-superJumbo.jpg?quality=75&auto=webp)


## DATA AND FILE OVERVIEW
The data folder, data/, contains two folders: raw/ and processed/. The structure of the data folder is as follows:

<pre> data/
├── processed/
│   ├── all_cover_fixed_Grazda.csv
│   ├── snow_cover.csv
│   └── species_presence.csv
├── raw/
│   ├── 01_ASDN_Readme.txt
│   ├── ASDN_Daily_species.csv
│   └── ASDN_Snow_survey/ </pre>

- `all_cover_fixed_Grazda.csv`: Cleaned snow survey data
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



## DATA-SPECIFIC INFORMATION 
**for data/processed/all_cover_fixed_Grazda.csv**
  
Number of variables: 11

Number of cases/rows: 42830

Variable List: 

| Column Name	| Definition |
| Site |	Four-letter code of site at which data were collected |
| Year	| Year in which data were collected |
| Date	| Date on which data were collected |
| Plot |	Name of study plot on which survey was conducted |
| Location |	Name of dedicated snow-survey location, if applicable |
| Snow_cover	| Percent cover of snow, including slush |
| Water_cover |	Percent cover of water |
| Land_cover |	Percent cover of exposed land |
| Total_cover |	Total sum (to check the above percents; should always sum to 100) |
| Observer |	Person who conducted the survey |
| Notes	| Any relevant comments on the survey |

### Missing data codes: NA

All non-numeric entries in the snow_cover column were replaced with NA (or with 0 when appropriate). Any negative values or values exceeding 100% were removed. The same cleaning steps were applied to the land_cover and water_cover columns. Afterwards, when the total_cover equaled 100, missing values in the individual cover columns were inferred by subtracting the known values from 100, ensuring that all cover types summed to 100%.

### Specialized formats or other abbreviations used:

- Code:	Site name	Location	Latitude	Longitude	Total Study Plot Area (ha)
- barr:	Barrow	Alaska, USA	71.3	-156.6	220.4
- burn:	Burntpoint Creek	Ontario, Canada	55.2	-84.3	63.0
- bylo:	Bylot Island	Nunavut, Canada	73.2	-80.0	723.6
- cakr:	Cape Krusenstern	Alaska, USA	67.1	-163.5	54.1
- cari:	Canning River Delta	Alaska, USA	70.1	-145.8	722.0
- chau:	Chaun River Delta	Chukotka, Russia	68.8	170.6	248.2
- chur:	Churchill	Manitoba, Canada	58.7	-93.8	866.9
- coat:	Coats Island	Nunavut, Canada	62.9	-82.5	1239.1
- colv:	Colville River Delta	Alaska, USA	70.4	-150.7	324.8
- eaba:	East Bay	Nunavut, Canada	64.0	-81.7	1205.5
- iglo:	Igloolik	Nunavut, Canada	69.4	-81.6	59.8
- ikpi:	Ikpikpuk	Alaska, USA	70.6	-154.7	174.1
- lkri:	Lower Khatanga River	Krasnoyarsk, Russia	72.9	106.1	270.9
- made:	Mackenzie River Delta	Northwest Territories, Canada	69.4	-135.0	667.3
- nome:	Nome	Alaska, USA	64.4	-164.9	90.1
- prba:	Prudhoe Bay	Alaska, USA	70.3	-148.6	120.0

## SHARING/ACCESS INFORMATION

SHARING/ACCESS INFORMATION

Licenses/restrictions placed on the data:
N/A

Links to publications that cite or use the data:
N/A

[NSF Arctic Data Center](https://arcticdata.io)

The original ASDN_Snow_Survey.csv can be found in the [bred-meds213-data-cleaning](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-data-cleaning/tree/main/data/raw) repository. This is a subset of the dataset hosted by the NSF Arctic Data Center.

**Citation**
Please acknowledge this dataset and the authors in any analysis, publication, presentation, or other output that uses these data. If you use the full dataset, we suggest you cite it as:

Lanctot, RB, SC Brown, and BK Sandercock. 2016. Arctic Shorebird Demographics Network. NSF Arctic Data Center. doi: INSERT HERE.

If you use data from only one or a few sites, we suggest you cite data for each site as per this example, using the corresponding site PIs as the authors:

Lanctot, RB and ST Saalfeld. 2016. Barrow, 2014. Arctic Shorebird Demographics Network. NSF Arctic Data Center. doi: INSERT HERE.

Note that each updated version of the full dataset has its own unique DOI.


## Additional Info

Data were not collected every year at all sites. Studies of the population ecology of these birds included nest-monitoring to determine the timing of reproduction and reproductive success; live capture of birds to collect blood samples, feathers, and fecal samples for investigations of population structure and pathogens; banding of birds to determine annual survival rates; resighting of color-banded birds to determine space use and site fidelity; and use of light-sensitive geolocators to investigate migratory movements. 

Data on climatic conditions, prey abundance, and predators were also collected. Environmental data included weather stations that recorded daily climatic conditions, surveys of seasonal snowmelt, weekly sampling of terrestrial and aquatic invertebrates that are prey of shorebirds, live trapping of small mammals (alternate prey for shorebird predators), and daily counts of potential predators (jaegers, falcons, foxes). Detailed field methods for each year are available in the `ASDN_protocol_201X.pdf` files. All research was conducted under permits from relevant federal, state, and university authorities.


See `01_ASDN_Readme.txt` provided in the [course data repository](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-spring-2024-class-data) for full metadata information about this data set.

