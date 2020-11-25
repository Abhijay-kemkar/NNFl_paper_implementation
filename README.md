# NNFl_paper_implementation

We Thank Prof. Bhanot and Prof Mukherjee for their teaching, knowledge sharing and guidance in the field of Neural Networks and Optimization.
We also thank Atharva Dubey for helping and guiding us throughout this project.
This project would not have been possible without the help of the aforementioned people.

The paper builds upon a elegant architecture “fully convolutional network”, modifies and extends this architecture such that it works with very few training images and yields more precise segmentations.The paper presents a network and training strategy that relies on the strong use of data augmentation to use the available annotated samples more efficiently for biomedical data segmentation.

Implementation of the paper **U-Net: Convolutional Networks for Biomedical Image Segmentation**
**link of the paper** : *https://arxiv.org/pdf/1505.04597.pdf*

**visulize.ipynb** : can be used for visualizing augmentation and elastic deformation, overlap tiling strategy, splitting into patches, weight maps generations. 

**Loading_HeLA_dataset.ipynb** : can be used for loading the HeLa dataset from given format to a format like one folder containng images and other folder containing segmentation masks in '.png' format 

**data.ipynb** : can be used for creating final numpy arrays which can be used for training the models. All types of preprocessing like augmentation, elastic deformation, overlapping tiling strategy can be implemented from this.

**Training_Unet.ipynb** : For training the Unet 

**Training_ResUnet.ipynb** : For training the ResUnet 

**Training_Weight_Map.ipynb** : For training the Unet along with pre-computed weight maps

**Future Work** :

1.We are training using pre-computed weight maps using a custom defined function  with the help of morphological operations but due to this the training process is very slow.     Hence in future we hope to optimise the custom defined function and then retrained.

2.We could explore different hybrid variation of U-Net like UNET++ and Attention U-Net, to achieve improved segmentation accuracy and model sensitivity.

3.Segmentation isn’t only used for medical images but also has application in a variety of other fields like earth sciences, remote sensing systems from satellite imagery and     autonomous vehicle systems. Hence, U-Net architecture can be applied to other segmentation tasks as well.This can also be applied in other areas such as quality control and     inspection and manufacturing.
