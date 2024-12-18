# Horse_diet
Metadata and code for free-roaming horse diet project

The following input csv files are read in and used with the R code "graminoid_composition.Rmd" and represent analyses that were conducted reflecting proportions of graminoids present in horse diets. 

File "9_10_24plant_family_percents_outputoftrnlcleaned.csv" shows the percentage of each plant family present in each sample. 
File "11_9_23_metadata_no_copy.csv" is the metadata regarding each individual fecal collection - location, HMA, time, and any known info about the horse the fecal material came from if defecation as observed
File "bcs_by_observation_5_24_23.csv" is the data regarding each body condition score observation
File "allHMAs_withRAP_4_18_24.csv" is the metadata for each HMA (provided by the BLM) with the spatially calculated RAP 2020 cover proportions and biomass values. These values represent the cover and biomass present through the spatial extent of each HMA  
File "5_9_23_metadata_no_copy_withRAP.csv" is the metadata for each individual fecal collection (as above) with columns added for spatially calculated RAP 2020 cover and biomass. These values represent the "potential movement buffers" of each individual horse to represent the theoretical available cover or biomass to that animal in the 36 hours preceeding fecal defecation.  

The code "graminoid_composition.Rmd" will take you through the steps to complete downstream analyses related to proportion of graminoids in the diet and include: seasonal comparisons of diet graminoid composition within each HMA and at the range-wide scale, seasonal comparisons of body condition within each HMA and at the range-wide scale, correlations between graminoid composition and herbacous cover and biomass, correlations between graminoid composition and body condition, and the figures to visualize these relationships.     
