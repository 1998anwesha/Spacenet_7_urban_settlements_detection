# Spacenet_7_urban_settlements_detection

Download the Spacenet 7 dataset from [here](https://spacenet.ai/sn7-challenge/).

### Objective: to perform binary segmentation of urban settlements from satellite imagery data

Spacenet – 7 dataset (has 10 million images) contains high resolution satellite imagery in TIF file format. It contains the spatio-temporal information (latitude /longitude and month/ time it was captured, area of interest). This dataset spans 24 months, with each region of interest represented by monthly TIF files. And in addition it also corresponding polygon geometries for every building captured in the TIF file — this can be used as our ground truth data). 

For training, We use the Unet architecture for generating binary masks.  Small chips of the original TIF files were created for feeding into Unet. Unet gives us the pixel wise labelling/classification, helps us figure out what every single pixel is in an image. 

