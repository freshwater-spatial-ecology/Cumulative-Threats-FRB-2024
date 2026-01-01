# Cumulative-Threats-FRB-2024

Data from: Iacarella, J.C., Paterson, K., Potapova, A., and Weller, J.D. 2025. Geospatial Indicators and Metrics for Threats to Fish Habitat in the Fraser River Basin with Thompson-Nicola as a Case Study.
DFO Can. Sci. Advis. Sec. Res. Doc. 2025/013. xiii + 126 p

Please refer to the report above for detailed methods or contact Keegan.paterson@dfo-mpo.gc.ca for questions. 

Individual and Cumulative threat scores were estimated for each BC Freshwater Atlas (BC FWA) stream “reach” within the Fraser River Basin (FRB) (i.e. fwa_watershed_code begins with 100). 
Stream “reaches” are identified by their “linear_feature_id”. 

The output feature class is stored in the geodatabase cumulative_threats_frb_ 2024.gdb. This current version includes the transformed and scaled threat scores as well as the cumulative human activity and climate change threat scores. All individual threat scores have values from 0-1, where 0 is the lowest threat and 1 is the highest threat score across the FRB. The cumulative threat scores are the sum of all individual threat scores. The feature class contains the original BC FWA attributes. Refer to the fwa_user_guide.pdf for information on the BC FWA. 

An updated version containing the raw threat scores (i.e. untransformed/normalized) and the RCP 8.5 climate change scores will be uploaded soon. Furthermore, we have modified and added several new human activity threat scores (e.g. disturbance to large-woody debris recruitment) that will be added to the database in the next update. 

Attributes:

ais_score – Aquatic invasive species threat score.  

anadfrag_score – Longitudinal fragmentation for anadromous species threat score. 

flowalt_score – Flow alteration threat score. 

habdest_score – In-stream habitat destruction threat score. 

latfrag_score – Latitudinal fragmentation threat score. 

resfrag_score – Longitudinal fragmentation for resident species.

ripdist_score – Riparian disturbance threat score. 

sed_score –  Sediment loading score derived from estimated sediment concentration from anthropogenic non-point sources (i.e. land use and cover).

nuts_score – Nutrient loading score derived from estimated nutrient concentrations from anthropogenic point and non-point sources (i.e. land use and cover).

poll_score – Pollutant loading score derived from estimated pollutant concentrations from point and non-point sources (i.e. land use and cover). 

ct_score – Human activity and landscape disturbance cumulative threat score. Calculated as the sum of all individual human activity/landscape disturbance threat scores (i.e. ais, anadfrag, flowalt, habdest, latfrag, resfrag, and ripdist). 

lowflow_score – Low flow threat score for 2040-2060 under RCP 4.5. Derived from the projected low minimum August %MAD-monthly stream flows. 

highflow_score –  High flow threat score for 2040-2060 under RCP 4.5. Derived from the projected high maximum May %MAD-monthly stream flows. 

floodrisk_score – Flood risk threat score for 2040-2060 under RCP 4.5. Derived based on projected absolute flood level change. 

hightemp_score – High stream temperature threat score for 2040-2060 under RCP 4.5. Derived from projected high August stream temperatures. 

cc_score – Climate change cumulative threat score. Calculated as the sum of all individual climate change threat scores (i.e. lowflow_score, hightemp_score, lowtemp_score). 
