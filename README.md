# W272-CA_leaflet
This code will run various .csv files with the overall goal of creating a leaflet map/html file for 
visualizng the state of California and specifically Los Angeles County. The map includes general 
aviation airports throughout the state that distribute both 100 and 100LL aviation gasoline (avgas), 
CA SB535 Disadvantaged Communities by census tract, and 2023 EPA Toxics Release Inventory (TRI) data
on lead and lead compound emitting facilities. 

Packages necessary are (some may not be used in the final product): 
  library(tidyverse)
  library(ggplot2)
  library(dplyr)
  library(MASS)
  library(sf)
  library(readr)
  library(here)
  library(stringr)
  library(ggspatial)
  library(gridExtra)
  library(tigris)
  library(tidygeocoder)
  library(leaflet)
  library(ggmap)
  library(paletteer)
  library(leaflet.extras)
  library(classInt)
  library(arcgisgeocode)
  library(mapview)
  library(htmlwidgets)

Data files include:
FAA-- filtered to CA and those that have 100 and 100LL avgas available
  100LL airport information
  100 airport information
EPA-- filtered to CA and for lead/lead compounds
  2023 TRI facilities 
CDPH-- listed by census tract only and de-identified
  2018-2022 Childhood Blood Lead Level Data
CalEPA-- 
  CalEnviroScreen4.0
  CA SB535
