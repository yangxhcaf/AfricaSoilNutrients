# SubSaharan Africa nutrient maps at 250 m resolution

Summary: This repository contains R code and some outputs of spatial predictions related with the production of soil macro and micro-nutrients maps for Sub-Saharan Africa at 250 m spatial resolution and for standard depth interval of 0–30 cm. Model training was run using soil samples from ca. 59,000 locations (a compilation of soil samples from the AfSIS, EthioSIS, One Acre Fund, VitalSigns and legacy soil data) and an extensive stack of remote sensing covariates, as well as landform, lithologic and land cover maps. For generating spatial predictions, an ensemble model from the machine learning algorithms random forest and gradient boosting, as implemented in R packages ranger and xgboost, was used. The results of cross-validation showed that apart from S, P and B, significant models can be produced for most targeted nutrients (R-square between 40–85 %). A limiting factor for mapping nutrients using the existing point data in Africa is high spatial clustering of sampling locations with many countries / land cover and land use groups completely unrepresented.

![alt text](https://github.com/ISRICWorldSoil/AfricaSoilNutrients/blob/master/plots/Fig_AfNutrients_final_maps_micro.png)
![alt text](https://github.com/ISRICWorldSoil/AfricaSoilNutrients/blob/master/plots/Fig_AfNutrients_final_maps_macro.png "Output predictions for micro and macro-nutrients.")

*Please cite as:*

* Hengl, T., Leenaars, J.G.B., Shepherd, K.D., Walsh, M.G, Heuvelink, G.B.M., Mamo, T. et al. (2017) [**Soil nutrient maps of Sub-Saharan Africa: assessment of soil nutrient content at 250 m spatial resolution using machine learning**](https://link.springer.com/content/pdf/10.1007/s10705-017-9870-x.pdf). Nutrient Cycling in Agroecosystems, DOI: 10.1007/s10705-017-9870-x.

# Download Maps

All maps are available for download under the [Open Database License (ODbl) v1.0](https://opendatacommons.org/licenses/odbl/) and can be downloaded from [www.isric.org](http://gsif.isric.org/doku.php/wiki:africa_nutrient_maps) without restrictions.

# Disclaimer

These are results of spatial predictions based on using Machine Learning algorithms attached to the above-listed paper and hence some errors and artifacts are still possible. We aim at updating these maps regularly i.e. as the new training / point data arrives. See also [ISRIC's general disclaimer](http://www.isric.org/data/data-policy/#disclaimer). Predictions of potential yield (e.g. [PotYield_crop1Maize_1km.tif](https://github.com/ISRICWorldSoil/AfricaSoilNutrients/blob/master/maps/PotYield_crop1Maize_1km.tif)) are based on the OFRA training data. These predictions are presented for experimental purposes only. 
