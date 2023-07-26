# CAR-violence-displacement-food-deprivation
This repository features an interactive map for the Central African Republic (CAR) with different layers for violent incidents from 2010-2023 (using ACLED data), food deprivation in 2023 (using IPC data) and internally displaced populations for 2023 (using manually compiled data from UMHCR reports). Note that the cutoff month and year are July 2023.

# Map layers
- Cities > 30k: locations of cities larger than 30k people according to 2012 estimates scaled according to the log of their estimated populations
- ACLED fatalities 2010-2023: violent incident locations scaled according to number of fatalities. The display of violent incidents can be adjusted under "Filters" according to the year, so that only a selected time-window of fatalities and their locations are shown
- 2023 new IDPs: newly displaced persons (aggregated from UMHCR reports for 2023) per sub-prefecture
- IPC percentage of population with crisis-level food insecurity: sub-prefectures are colored (bright to dark according to increasing severity) according to number of people; IPC defines crisis-level as level 3 or higher. IPC gives 5 total ordinal levels: 1-Minimal ; 2-Stressed ; 3-Crisis ; 4-Emergency ; 5-Famine
- IPC food insecurity affected number of people: sub-prefectures are colored (bright to dark according to increasing severity) according to number of people with level 3 or higher levels of food insecurity according to IPC (for level classification see above)
-  IPC crisis-level food insecurity: sub-prefectures are colored (bright to dark according to increasing number) according to IPC's overall estimation of the food insecurity in the sub-prefecture given as an ordinal integer using IPC food insecurity levels (for level classification see above)
