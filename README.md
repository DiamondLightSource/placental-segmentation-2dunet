# placental-segmentation-2dunet

This repository contains Jupyter Notebooks and data for the training of 2d U-net models on placental blood vessel and maternal/fetal blood volume data. In addition separate notebooks allow the application of the trained U-net models to 3d blocks of image data in order to produce segmented outputs. 

## Blood vessel 2d U-net training

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DiamondLightSource/placental-segmentation-2dunet/blob/main/blood_vessels/placenta_blood_vessel_2d_unet_training.ipynb)
- A Jupyter Notebook which enables slicing of a 3d region of placental blood vessel data into image stacks in the 3 planes parallel to  *xy*, *xz* and *yz*. This is followed by training of a 2d U-net on these images. 

## Blood vessel 2d U-net prediction

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DiamondLightSource/placental-segmentation-2dunet/blob/main/blood_vessels/placenta_blood_vessel_2d_unet_prediction.ipynb)
- A Jupyter Notebook which enables slicing of a 3d region of placental blood vessel data into image stacks in the 3 planes parallel to  *xy*, *xz* and *yz*. This is followed by prediction of the segmentation of these images using a 2d U-net before recombining the images into 3d volumes. The image data is then rotated by 90 degrees around the 4-fold symmetry axis running perpendicular to the *xy* plane and the entire slicing and prediction process repeated again. This happens 4 times, before the 12 resulting output volumes are combined.  

## Maternal/Fetal blood volume 2d U-net training

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DiamondLightSource/placental-segmentation-2dunet/blob/main/maternal_fetal_blood_volumes/maternal_fetal_blood_vol_2d_unet_training.ipynb)
- A Jupyter Notebook which enables slicing of a 3d region of maternal/fetal blood volume data into image stacks in the 3 planes parallel to  *xy*, *xz* and *yz*. This is followed by training of a 2d U-net on these images.

## Maternal/Fetal blood volume 2d U-net prediction

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/DiamondLightSource/placental-segmentation-2dunet/blob/main/maternal_fetal_blood_volumes/maternal_fetal_blood_vol_2d_unet_prediction.ipynb)
- A Jupyter Notebook which enables slicing of a 3d region of maternal/fetal blood volume data into image stacks in the 3 planes parallel to  *xy*, *xz* and *yz*. his is followed by prediction of the segmentation of these images using a 2d U-net before recombining the images into 3d volumes. The image data is then rotated by 90 degrees around the 4-fold symmetry axis running perpendicular to the *xy* plane and the entire slicing and prediction process repeated again. This happens 4 times, before the 12 resulting output volumes are combined.  