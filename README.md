## Image depth and planar regions

### Authors

* **Deepak Hazarika** 
* **Parinita Bora**
* **Gurudatta**

11/1/2020 8:55:19 PM 
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

was run on the above dataset.

All the 3590 images were placed in the input folder and the model weight was placed in the/midas/MiDaS-master folder.

The output is stored in midas_depth.zip in google drive

[https://drive.google.com/drive/folders/1sYmxMC_eU_1tWsAK5FceagzEfg49oyf9?usp=sharing](https://drive.google.com/drive/folders/1sYmxMC_eU_1tWsAK5FceagzEfg49oyf9?usp=sharing "midas image depth store")



# Planar region

The following model

[https://github.com/NVlabs/planercnn](https://github.com/NVlabs/planercnn "Planar region")

 was run on the above data set to generate the planar regions.

The pre -requisites for running this model are

- cuda 8.0
- gcc 5
- pytorch 0.4.0 / 0.4.1
 
A setup script was provided by one of the group member to setup the environment.

### What the script does?

Install cuda 8.0 , gcc 5 version

then compile plannercnn files , for this torch version 0.4.0 is required.Once done , remove torch 0.4.0 version and install 0.4.1.

### Evaluate

The images were split into smaller sets of 500 images and the model was used to generate the planar region.

#### Configuration

Before each run --numTestingImages parameter is set to 500 in options.py file.


### Post processing

Since 8 different subset of output were generated , the image files were renamed and then put in a common location.The generated files are stored in google drive as planar_region.zip

[https://drive.google.com/drive/folders/1sYmxMC_eU_1tWsAK5FceagzEfg49oyf9?usp=sharing](https://drive.google.com/drive/folders/1sYmxMC_eU_1tWsAK5FceagzEfg49oyf9?usp=sharing "midas image depth store")





 

   

