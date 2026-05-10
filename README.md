# Predicting-Stars---Quasars---Galaxies-
This project focuses on classifying astronomical objects into three categories: Stars, Galaxies, and Quasars using machine learning techniques.
The dataset used in this project is obtained from the Sloan Digital Sky Survey (SDSS) and contains photometric and spectroscopic measurements of celestial objects.
The goal of the model is to learn patterns from astronomical observations and automatically determine the type of object based on its measured features.

## Dataset Description
The dataset (Skyserver_SQL.csv) contains 10,000 astronomical observations with 18 features. Each row represents a celestial object detected by the SDSS telescope.
These features include positional information, photometric measurements across multiple wavelengths, and spectroscopic identifiers.

Target Variable --> class

This is the label the model predicts. It has three categories:

    - STAR : Objects that emit light due to nuclear fusion in their cores.
    
    - GALAXY : Massive systems containing billions of stars, gas, and dust.
    
    - QSO (Quasar) : Extremely luminous active galactic nuclei powered by supermassive black holes.

## Feature Description

### Object Identifiers

objid : Unique identifier for the astronomical object in the SDSS database.

specobjid : Unique identifier for the spectroscopic observation.

### Positional Features
These describe the object’s location in the sky.

ra (Right Ascension) : Angular distance measured eastward along the celestial equator.

dec (Declination) : Angular distance north or south of the celestial equator.
