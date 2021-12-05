# Integration between OSM and authoritative data

This repository contains some information and outputs related to the project "Evaluation of Novel approaches for governing (location) data and technology. Combined use of public sector and citizen-generated data" financed by the European Commission - Joint Research Centre (JRC) that had, as main goal, the investigation of how authoritative and citizen-generated location data can be combined to support data-driven innovation and the European strategy for data.

After a first evaluation of the two datasets and the efforts required to perform the integration, the analysis focused on the addresses datasets only, as first example to analyse and discuss possible integration between authoritative and citizen-generated data.
In this project, the analysis is limited to a restricted geographical area—and not the whole Europe—and specifically Finland and the Netherlands were identified as investigated use cases.

## Data sources

The project re-used already existing data, namely from the National Land Survey (NLS) of Finland (https://www.maanmittauslaitos.fi/en) and the Dutch cadastre of addresses and buildings as authoritative data, and OpenStreetMap (OSM) as citizen-generated data.

The National Land Survey (NLS) of Finland provides various services to access and download address datasets both via standard OGC and INSPIRE services, more recent OGC API- Features (as a beta and not fully supported service), as well as modern encodings like GeoPackage. Data were downloaded from the following OGC API-Feature service: https://beta-paikkatieto.maanmittauslaitos.fi/inspire-addresses/features/v1

Dutch data are provided by the Dutch cadastre of addresses and buildings (BAG: Basisregistratie Adressen en Gebouwen1) and were downloaded as a csv file from https://geotoko.nl, a webshop portal that sells processed national datasets, but provide them for free for open data projects like OSM.

OpenStreetMap (OSM) data were extracted from the [Planet OSM](https://planet.openstreetmap.org)

## Data analysis

Some ETL processes and test data are present to allow the reproducibility of the integration between OpenStreetMap data and authoritative data.

In particular, currently contains 3 ETL processes developed using the [QGIS graphical modeler](https://docs.qgis.org/3.16/en/docs/user_manual/processing/modeler.html) to combine addresses data in Finland and a test dataset of integrated addresses for the city of Helsinki.

## Licences

Source datasets are available as open data, with different licenses applied:
* Finland NLS data on addresses and buildings: Creative Commons Attribution 4.0 International (https://creativecommons.org/licenses/by/4.0/)
* BAG data are Pubic Domain data (https://creativecommons.org/publicdomain/mark/1.0/deed.en)
* OpenStreetMap data: Open Data Commons Open Database License (ODbL) (https://opendatacommons.org/licenses/odbl/)

The licences adheres to the [Open Definition](http://opendefinition.org/), with the CC-BY requiring only attribution, while the ODbL requiring, in addition, the redistribution with the same licence (Share-Alike clause). For this reason, derived datasets produced by the integration of the original sources (NLS, BAG and OSM) are released under the ODbL, to allow full reusability by third parties.

## Integrated datasets

The integrated datasets produced after the analysis are deposited in Zenodo, allowing a full preservation and citability (using assigned DOI), and are accessible at the following URLs:
* Finland: https://doi.org/10.5281/zenodo.5735492
* Netherlands: https://doi.org/10.5281/zenodo.5740441
