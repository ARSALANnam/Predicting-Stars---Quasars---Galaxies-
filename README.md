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

### Photometric Measurements in Five Bands (u, g, r, i, z)

In astronomical surveys such as the Sloan Digital Sky Survey (SDSS), objects are observed using five different photometric filters: u, g, r, i, and z. These filters measure the brightness of celestial objects at different ranges of the electromagnetic spectrum.

Each band corresponds to a specific wavelength range of light:

    u-band (ultraviolet) – measures light in the near‑ultraviolet region (~354 nm).
    g-band (green) – captures light in the blue‑green part of the spectrum (~477 nm).
    r-band (red) – measures red visible light (~623 nm).
    i-band (near‑infrared) – captures light slightly beyond the red part of the spectrum (~763 nm).
    z-band (infrared) – measures deeper near‑infrared wavelengths (~913 nm).

The values recorded in these columns represent the magnitude, which is a logarithmic measure of an object’s brightness. In the magnitude scale, smaller numbers correspond to brighter objects, while larger numbers indicate fainter objects.

Using measurements from these five bands allows astronomers to study the color and physical properties of astronomical objects. Differences between magnitudes in different bands (for example, u − g or g − r) are called color indices, and they provide important information about temperature, composition, and redshift.

These photometric features are also very useful in machine learning and classification tasks, because different types of astronomical objects—such as stars, galaxies, and quasars—tend to have distinct brightness patterns across the five bands.

### Observation Metadata

These columns describe the telescope imaging configuration.

    run – Imaging run number
    rerun – Data processing rerun number
    camcol – Camera column used for observation
    field – Field number of the observation

### Spectroscopic Information

These features are related to spectral measurements.

redshift : Measures how much the wavelength of light from the object has shifted due to cosmic expansion.
Higher redshift typically indicates objects that are farther away (often quasars or distant galaxies).

plate : Spectroscopic plate identifier.

mjd : Modified Julian Date of observation.

fiberid : Fiber number used during spectroscopic observation.


## Dataset Source
https://www.kaggle.com/datasets/lucidlenn/sloan-digital-sky-survey/discussion?sort=hotness
