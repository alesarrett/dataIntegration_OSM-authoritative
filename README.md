# Integration between OSM and authoritative data

This repository contains some ETL processes and test data to describe an exercise of integration between OpenStreetMap data and authoritative data.

In particular, currently contains 3 ETL processes developed using the [QGIS graphical modeler](https://docs.qgis.org/3.16/en/docs/user_manual/processing/modeler.html) to combine addresses data in Finland and a test dataset of integrated addresses for the city of Helsinki.

Authoritative data comes from the National LandSurvey  (NLS)  of  Finland  (https://www.maanmittauslaitos.fi/en) through the OGC API - Features service endpoint, accessed from the [New Address Information System](https://www.maanmittauslaitos.fi/osoitetietojarjestelma): https://beta-paikkatieto.maanmittauslaitos.fi/inspire-addresses/features/v1
The NLS address dataset is available under the [CC BY 4.0 license Creative Commons](https://creativecommons.org/licenses/by/4.0).

OpenStreetMap (OSM) data were extracted from the [Planet OSM](https://planet.openstreetmap.org), downloaded on 7 June 2021.

In the test dataset, the original data source is documented in the field "source", with the two values "OSM and "NLS".
