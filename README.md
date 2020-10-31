## Image depth and planar regions

### Authors

* **Deepak Hazarika** 
* **Parinita Bora**
* **Gurudatta**

10/31/2020 11:53:40 PM 
----------

## Dataset

3590 images having the following objects

- Hardhat
- Mask
- Vest
- Boots

were collected by the EVA5 group.
 

# Image depth

The following model: 

[https://github.com/intel-isl/MiDaS](https://github.com/intel-isl/MiDaS "image depth") 

was run on the above dataset.The output is stored in midas_depth.zip in this repository


# Planar region

The following model

[https://github.com/NVlabs/planercnn](https://github.com/NVlabs/planercnn "Planar region")

 was run on the above data set to generate the planar regions.The pre -requisites for running this model are

- cuda 8.0
- gcc 5
- pytorch 0.4.0 / o.4.1
 

The output is stored as planar_region.zip in this repository.  

