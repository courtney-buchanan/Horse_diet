# Horse_diet
Metadata and code for free-roaming horse diet project

The code "trnl_cleaned_up.Rmd" uses the taxonomy assignment and read count files output from the bioinformatics pipeline to prepare the diet composition information for data analysis. Among other processing steps, read counts are filtered to exclude rare taxa, grouped by family, and outputed to be used for further analyses of graminoid composition of diets. Visualizations of diet composition by familiy are also created for the range as a whole, for each HMA, and also for each individual within each HMA. 

The following input csv files are read in and used with the R code "trnl_cleaned_up.Rmd".

File "1_31taxonomy.csv" is the taxonomy assingned to each ASV (amplicon sequence varaint)

File "renamed_1_31_read_table_no_plants.csv" is the read count for each ASV within each fecal collection, but does not include plant taxonomy. There are two copies of read counts for each fecal collection that was submitted. This was too large a file to upload and so is uploaded in two files that can be combined. The original file was 985 rows and is broken into two: The first file "renamed_1_31_read_table_no_plants1-503summer.csv" contains read counts for all the summer fecal collections and the second file "renamed_1_31_read_table_no_plants504-985winter.csv" contains all the read counts for the winter fecal collections. Both files have the heading containing the ASV sequences.  

File "5_4_23_hore_fecal_metadata.csv" is the metadata for each individual fecal collection- location, HMA, time, and any known info about the horse the fecal material came from if defecation as observed.  This file has two copies of the metadata to align with the original read data that had two copies for each fecal collection. These two copies were later merged.  

File "11_9_23_metadata_no_copy.csv" is the same metadata as above regarding each individual fecal collection, now with a single copy to align with the merged data. 

This code will ouput the file "9_10_24plant_family_percents_outputoftrnlcleaned.csv" which is the diet composition for each fecal collection grouped at the family taxonomic level which is used in the analyses below..

The code "graminoid_composition.Rmd" goes through the steps to complete downstream analyses related to the graminoid composition in the horse diets and includes: seasonal comparisons of diet graminoid composition within each HMA and at the range-wide scale, seasonal comparisons of body condition within each HMA and at the range-wide scale, correlations between graminoid composition and herbacous cover and biomass, correlations between graminoid composition and body condition, and the figures to visualize these relationships. There are also some additional analyses related to select other plant families as well. 

The following input csv files are read in and used with the R code "graminoid_composition.Rmd". 

File "9_10_24plant_family_percents_outputoftrnlcleaned.csv" shows the percentage of each plant family present in each individual fecal collection. 

File "11_9_23_metadata_no_copy.csv" is the metadata regarding each individual fecal collection - location, HMA, time, and any known info about the horse the fecal material came from if defecation as observed. 

File "bcs_by_observation_5_24_23.csv" is the data regarding each body condition score observation made. 

File "allHMAs_withRAP_4_18_24.csv" is the metadata information for each HMA (provided by the BLM) with the spatially calculated RAP 2020 cover proportions and biomass values. These values represent the cover and biomass present through the spatial extent of each HMA.  

File "5_9_23_metadata_no_copy_withRAP.csv" is the metadata for each individual fecal collection with columns added for spatially calculated RAP 2020 cover and biomass. These values represent the "potential movement buffers" of each individual horse to represent the theoretical available cover or biomass to that animal in the 36 hours preceeding fecal defecation.  

  
