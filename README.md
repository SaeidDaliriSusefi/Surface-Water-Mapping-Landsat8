# Water Body Detection

This repository contains code for processing Landsat 8 imagery to calculate the Normalized Difference Water Index (NDWI) and apply K-Means clustering to identify water bodies within a defined region of interest (ROI) and desired period of time.








![image alt](https://github.com/SaeidDaliriSusefi/Water-Body/blob/483c6aaef4a41999612a054585491e7348f92ffc/Images/Examples.jpg)



### Features:
NDWI Calculation: Computes the NDWI index using Landsat surface reflectance bands (SR_B3 and SR_B5).

Cloud and Shadow Masking: The code includes cloud, cirrus, and shadow masking using the QA_PIXEL band to ensure that the NDWI values are accurate.

K-Means Clustering: After calculating the mean NDWI, K-Means clustering is applied to distinguish between water and non-water areas.

Water Body Area Calculation: The code estimates the area of water bodies in square kilometers based on the clustering results.

Visualization: It generates a plot of the mean NDWI and the identified water bodies, along with the calculated water body area.



### Requirements:
Google Earth Engine (GEE): The code uses the Earth Engine Python API to access and process Landsat imagery.

xarray: For handling multidimensional data (e.g., raster datasets).

matplotlib: To plot the results.

scikit-learn: For applying the K-Means clustering algorithm.
