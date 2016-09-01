##ANOMALY DETECTION AND SUMMARISATION OF VARIOUS EXTREME WEATHER EVENTS OVER THE INDIAN SUB-CONTINENT
###Introduction
This repository contains all the R codes that I have written during my summer internship at IIT Kharagpur.
Project name : Anomaly detection and Summarisation of various extreme weather events over Indian sub-continent
The data that is dealt with is a spatio-temporal climate over the Indian sub-continent.

###Abstract
Anomalous weather events occur very rarely but they have a huge impact on human life. The aim of this study is to characterise the anomalous weather events over the Indian sub-continent using the climatological variables(surface air temperature, uwind, vwind,relative humidity and omega), so that their period of occurrence and their trajectory can be more accurately predicted, at a nascent stage. In this study, we use the Seasonal Hybrid Extreme Studentized Test to detect outliers during the period 1951 to 2014. It is most appropriate as it considers both the seasonal and trend aspect of the temporal, univariate data and is also highly robust in the presence of anomalies. The naive spatio-temporal clustering is used to aggregate the anomalies, based on their spatial and temporal context, which are later used to evaluate and also validate the anomaly detection technique. The cSTAG algorithm is then used to discover regions of correlated spatio-temporal change, so that wecan first separate and then characterise the events that caused them. The results are visualised over the map of India and we find that it aptly portrays the evolution of a particular event over consecutive days. These results can be used by domain experts to better study the
behavior of these extreme events. Through this project, we have been able to detect extreme weather events like heat waves, rainstorms over the Indian sub-continent as well as validated it with real-time data. Weather events like floods,fog are not detected by the method that we used. Due to lack of data regarding reported cold wave events, a large number of them cannot be validated.

###Dataset description
The weather data used for the study is collected from the NCEP/NCAR website and was downloaded from [data](www.esrl.noaa.gov/psd/data/gridded/data.ncep.reanalysis.pressure.html) in NetCDF format. The atmospheric variables : surface air temperature, uwind, vwind, relative humidity and omega, provided at the pressure level of 925 hPa was downloaded in separate files. The dataset contain records taken from 1 st January,1951 to 31 st December, 2014. It covers the area from 5°N to 40°N and from 65°E to 100°E. Each grid has a spatial coverage of 2.5° x 2.5°.
####Global attributes:
  1. conventions = “COARDS”
  2. Description = Data is from NMC reanalysis (4 times/day). It consists of most variablesinterpolated to pressure surfaces from model(sigma) surfaces.
