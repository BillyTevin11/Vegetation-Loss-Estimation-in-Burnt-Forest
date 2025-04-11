
![download](https://github.com/user-attachments/assets/50a65551-e263-4025-b754-541d4d7399dd)


# <ins>Vegetation Loss Estimation in Burnt Forest, Uasin Gishu County</ins>

The project focuses on assessing vegetation loss due to fires in **Burnt Forest**, Uasin Gishu County, Kenya, using satellite imagery and remote sensing techniques. Implemented in a Jupyter Notebook environment and leveraging the power of Google Earth Engine (GEE), this analysis utilizes Landsat 8 and 9 Level 2 Collection 2 Tier 1 imagery to monitor changes in vegetation over time.

The primary objective is to estimate the extent of vegetation cover lost during a fire event in early 2019. The workflow begins by defining the area of interest (AOI) using FAO's GAUL administrative boundaries dataset, specifically filtering for Uasin Gishu County. High-quality satellite images with minimal cloud cover from January to March 2019 are selected to represent pre- and post-fire conditions.

A key step in the process is the calculation of the _Normalized Difference Vegetation Index (NDVI)_, which is used to assess vegetation health. NDVI values are computed for each image in the Landsat collection, and median composites are generated for pre-fire (January 2019) and post-fire (late February to March 2019) periods.

The difference between the pre- and post-fire NDVI images highlights areas of vegetation loss. This NDVI change map is further processed using Simple Non-Iterative Clustering (SNIC) segmentation to enhance spatial coherence in the imagery. By applying a threshold of **0.15** to the NDVI change values, areas that experienced significant vegetation loss are identified and quantified.

The analysis concludes by calculating the total area of vegetation loss in square kilometers using pixel-based area estimation. Finally, the segmented NDVI data is visualized using XArray and Matplotlib, providing clear visual comparisons of vegetation conditions before and after the fire. Outputs include NDVI maps and threshold visualizations, which are saved as high-resolution images for reporting or presentation purposes.

Overall, this project demonstrates a practical and scalable approach to monitoring fire impacts on vegetation using open-source tools and satellite data.





