# CAR-violence-displacement-food-deprivation
This repository features an interactive map for the Central African Republic (CAR) with different layers for violent incidents from 2010-2023 (using ACLED data), food deprivation in 2023 (using IPC data) and internally displaced populations for 2023 (using manually compiled data from UMHCR reports). Note that the cutoff month and year are July 2023.

# Map layers
- Cities > 30k: locations of cities larger than 30k people according to 2012 estimates scaled according to the log of their estimated populations
- ACLED fatalities 2010-2023: violent incident locations scaled according to number of fatalities. The display of violent incidents can be adjusted under "Filters" according to the year, so that only a selected time-window of fatalities and their locations are shown
- 2023 new IDPs: newly displaced persons (aggregated from UMHCR reports for 2023) per sub-prefecture colored (bright to dark according to increasing severity) according to number of people
- IPC percentage of population with crisis-level food insecurity: sub-prefectures are colored (bright to dark according to increasing severity) according to number of people; IPC defines crisis-level as level 3 or higher. IPC gives 5 total ordinal levels: 1-Minimal ; 2-Stressed ; 3-Crisis ; 4-Emergency ; 5-Famine
- IPC food insecurity affected number of people: sub-prefectures are colored (bright to dark according to increasing severity) according to number of people with level 3 or higher levels of food insecurity according to IPC (for levels classification see above)
-  IPC crisis-level food insecurity: sub-prefectures are colored (bright to dark according to increasing number) according to IPC's overall estimation of the food insecurity in the sub-prefecture given as an ordinal integer using IPC food insecurity levels (for levels classification see above)

# Notes
There are weak but significant correlations between sub-prefectural averaged levels of food deprivation (Spearman rank=0.29, p=0.038; I averaged the different food insecurity level-percentages of affected persons per subprefecture for a finer-grained picture than the IPC overall food insecurity estimate) and 2023 sub-prefectural aggregated fatalities as well as between 2023 sub-prefectural aggregated fatalities and 2023 sub-prefectural numbers of recently internally displaced persons (Spearman rank=0.3, p=0.032). Displacement and food deprivation were not correlated.

However, a longer term country-level comparison between 3-year-averages of total fatalities in CAR (based on ACLED) and undernourishment data from the Food and Agriculture Organization of the United Nations (FAO) from 2000-2022 results in a strong and highly significant correlation (Pearson=0.8048057033599774, p=1.09 × 10-5). The results using the Uppsala Conflict Data Program are very similar with Pearson=0.7788435997908856, p=3.19 × 10-5 (Spearman is even higher with 0.8181818181818182, pvalue=5.853154433552813 × 10-6).
