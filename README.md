# csem-api

## 3D Marine Controlled Source Electromagnetic modeling API

This API is designed for modelling of marine CSEM data in time and frequency domain on a remote cluster/cloud service. It may be used for feasibility and interpretation work on EM data with Jupyter Notebook.  

A 3D CSEM online modelling service supporting the API is available at https://api.geotech.no and provided by [GeoContrast AS](http://www.geocontrast.no) on AS-IS basis during trial period. You may request a free trial API key by sending an email with a short description of your use case to contact form at http://www.geocontrast.no 
Run the tutorial now in your browser: [![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/geocontrast/csem-api/master)

## Current features provided by https://api.geotech.no :

| Current version features | Available  | 
| --- | --- |
| Layered model | Yes | 
| Embedded boxes | Yes | 
| Resistivity depth gradient | No | 
| Spline horizons | No | 
| Frequency domain | Yes |
| Time domain | No |
| Anisotropy VTI | No |
| Anisotropy TTI | No |
| Magnetic field | No |


This simple models can be useful for feasibility studies, survey parameter testing, and some basic data analysis.

## Freqency domain

The geophysical model is defined in right-handed Cartesian coordinate system with Z axis pointing down. z=0 sea surface equal to the top of the first layer. All units are in SI. The source is horizontal electric dipole with given length with its center coordinates (0,0,source_layer_base-source_altitude) and aligned along X axis.

## Model limits

| Parameter limit | Lower  |  Higher |
| --- | --- | --- |
| Source receiver distance | 0 | 15000 |
| Number of receivers  | 1 | 1000 |
| Frequency | 0.1 | 5.0 |
| Resistivities | 0.2 | 1000 |
| Layer thinckness | 50 | 2000 |
| Box width | 50 | 5000 |
| Box thickness | 50 | 1000 |
| Number of boxes | 0 | 3 |
| Source length | 100 | 400 |

## Documentation

The API is documented by the set of Jupyter Notebook tutorials published in this repository

## Copyright

Copyright 2018 Geocontrast AS, Oslo, Norway









