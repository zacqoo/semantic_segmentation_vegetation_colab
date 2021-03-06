# semantic_segmentation_vegetation_colab
U-Net trained on satellite imagery/ drone imagery to segment aquatic vegetation on the river and lakes

Keras implementation, TensorFlow backend

## Introduction
In this project, we apply [U-Net](https://lmb.informatik.uni-freiburg.de/people/ronneber/u-net/) for semantic segmentation task on satellite imagery and drone imagery. We segment the aquatic vegetations, called "ceratophyllum" related to schistosomiasis in Senegal, Africa. Cerayophyllum appears to be dark blue color floating on rivers and lakes on drone and satellite images. From the segmentation, we are able to create maps of disease hotspot to evaluate infection risks in the area to better inform local disease control authority and make disease control more efficient.

## Code
See Colab (Jupyter) notebooks "main_keras_flow.ipynb" for more details. The code can be used for other objects in satellite/ drone images.

## Create masks
We use [Labelbox](https://www.labelbox.com/) to create mask on target vegetation features, as a team effort. Labelbox allows multiple users to label/ create masks on the images together. (*Most masks were made by Lance Lamore.)

![sample_1.jpeg](sample_1.jpeg)
![sample_1_mask.png](sample_1_mask.png)

## Pre-trained model
We also utilized VGG16 for training the model. See "main_keras_vgg16.ipynb" for U-Net and VGG16 architecture.

## Requirements
- Python 3
- Keras 2
- TensorFlow 1.2

(already installed with Google Colab environment)

## Sample images and segmentation (in red)

![drone_sample.JPG](drone_sample.JPG)
![drone_seg_sample.png](drone_seg_sample.png)

## Team
Zac Liu, Lance Lamore, Andy Chamberlin from Stanford University
