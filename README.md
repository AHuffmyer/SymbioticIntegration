# Study overview   

This repository contains data and scripts for an experiment testing the effects of temperature on coral-symbiont nutritional exchange in *Montipora capitata* larvae from summer 2021 in Hawaii.  

In this study, we exposed larvae of *M. capitata* to 3 days of +2.5°C temperatures above ambient. We collected data on larval survival, settlement, physiology, and metabolic response to temperature treatments. 

<img width="469" alt="Screenshot 2024-05-21 at 14 54 24" src="https://github.com/AHuffmyer/SymbioticIntegration/assets/32178010/c474484c-acb1-4b71-8bb3-85a80a35efb4">

In this study, we used stable isotope 13C carbon tracing metabolomics to understand metabolic responses to temperature treatment and track symbiotic nutritional exchange. An overview of these data types can be viewed below.  

<img width="520" alt="Screenshot 2024-05-21 at 14 54 31" src="https://github.com/AHuffmyer/SymbioticIntegration/assets/32178010/092598cc-dc5d-47d2-a443-f55376607608">

# Repository contents 

## Mcap2021

### Data 

Data is organized in the following sub directories:  

- `Carbohydrates`: Contains data for analysis of larval carbohydrate content. 
- `Cells`: Contains data for analysis of larval symbiont cell densities. 
- `Chlorophyll`: Contains data for analysis of larval chlorophyll content.
- `Environmental`: Contains data for environmental data including daily measurements, temperature data loggers, and data during metabolomics incubations.  
- `Metabolomics`: Contains data for analysis of larval metabolomics including stable isotope metabolomic data (`metabolite_data.xlsx`), metadata (`metabolomics_metadata.xlsx`), and time series methodological control (`timeseries_validation_data.xlsx`).  
- `Protein`: Contains data for analysis of larval total soluble protein.
- `Respiration`: Contains data for analysis of larval respiration and photosynthesis including metadata (`Resp_Sample_Info.csv`), start and end time data for measurements (`starttimes.csv`), and raw oxygen files contained in the `Runs` sub directory. Files are also included in Excel versions in the `Excel versions` sub directory.  
- `Size`: Contains data on larval size measurements generated through ImageJ analysis.  
- `Resuspension_volumes.csv` contains data on resuspension volumes for samples used for physiological analyses.  
- `Settlement.csv` contains data on larval settlement. 
- `Survivorship.csv` contains data on larval survivorship.  

Data is analyzed using the scripts listed below. Each script contains descriptions on analysis steps for each data type.  

### Scripts

This folder contains R scripts used in analysis for this study.   

`daily_measurement_analysis.Rmd`: Analysis of daily environmental measurements.   

`Larval_size.Rmd`: Analysis of larval size during the study.   

`metabolomics.Rmd`: Analysis of stable isotope tracing metabolomic data including pool size, enrichment, and carbon-specific enrichment data types and methodological controls.   

`Physiology.Rmd`: Analysis of larval physiology including symbiont cell density, symbiont chlorophyll content, carbohydrate content, and total protein for normalization.  

`Respirometry_Extraction.Rmd`: Extraction of metabolic rates from oxygen data for analysis of respiration and photosynthetic rates using localized linear regressions.  

`Respirometry_Plotting.Rmd`: Analysis of respiration and photosynthetic rates. 

`Settlement.Rmd`: Analysis of larval settlement.  

`Survivorship.Rmd`: Analysis of larval survival.

`Temperature_analysis.Rmd`: Analysis of temperature data collected from data loggers.  

`timeseries_metabolomics_validation.Rmd`: Analysis of time series metabolomic methodological controls.  

### Figures

This folder contains figures generated by the scripts listed above organized into the following sub directorires:  

- `Metabolomics`: Contains figures generated by metabolomic analyses.  
- `Respiration`: Contains figures generated by respiration rate extraction and analysis.  

Figures for larval survival, size, settlement, physiology, and temperature analyses are located in the main `Figures` directory.  

### Output

This folder contains output data frames and statistical output generated by the scripts listed above organized into the following sub directorires:  

- `Cells`: Contains output data of calculated symbiont cell density in larval samples.  
- `Metabolomics`: Contains output data and statistical results from metabolomics analyses, including lists of VIP metabolites and summary statistics.  
- `Protein`: Contains output data of calculated total soluble protein in larval samples.  
- `Respiration`: Contains output data of calculated respiraiton and photosynthesis rates in larval samples.  

Calculated larval size is output into the main `Output` directory.  

## Notebooks

This folder contains .md5 files of electronic notebook entries. 

# Raw data storage 

Raw metabolomics data files (.raw and .mzXML files) can be found at: DOI 10.17605/OSF.IO/TE6S2  

# Contact 

Contact Ariana Huffmyer (ashuffmyer (at) uri.edu) with questions or inquiries.  