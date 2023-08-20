# VC
Rainfall prediction in the Mondego river basin using CV and DL

# Introduction 
This project was delivered for the course unit "Computer Vision" of the Master in Data Science and Engineering.
It was a group project, which required from us to use deep learning and computer vision to predict the rainfall over a river basin. The objective of the project was to estimate the rainfall depth in a river basin, using weather forecasts/reanalysis datasets.

# Solution 
The project comprised the following steps:
1. Compute daily rainfall in the Mondego river basin using the Thiessen method.
   
   1.1. Create Thiessen construction for Portuguese basins
   
   1.2. Identify which Thiessen polygons intersect Mondego river basin
   
   1.3. Download data from SNIRH for period 1950 2021
   
   1.4. Load data to dataframes.
   
   1.5. Verify missing values
   
   1.6. Eliminate weather stations with too many missing values
   
   1.7. Reconstruct Thiessen polygons with validated weather stations
   
   1.8. Compute the spatial average of the rainfall in the Mondego RB
   
1. Create ECMWF meteorological dataset (tp, tcc, t2m)

2.1. Define coordinates (lat/long) for download

2.2. Download data from ECMWF for period defined in 1.7

2.3. Convert lat/long to Carthesian coordinates (EPSG:3763)

2.4. Generate images (rainfall, temperature, total cloud coverage)
   
1. Develop CNN for spatial averaged rainfall prediction

3.1.Dataset preprocessing

3.2. Data loader

3.3. CNN model

3.4. Training routine

3.5. Evaluation routine

3.6. Hyper parameter tunning

3.7. Testing different image sizes

3.8. Results evaluation


# Contributions
João Pedro Pêgo, Pedro Gouveia, Kareem Kousa
