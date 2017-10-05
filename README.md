# mDRFI _ Matlab
Saliency detection in dermoscopic images
===========

Saliency detection in dermoscopic images as described in this paper: "Supervised Saliency Map Driven Segmentation of the Lesions in Dermoscopic Images" by M. Jahanifar et al.(arXiv: https://arxiv.org/abs/1703.00087)

** This is a part of an algorithm for lesion segmentation in dermoscopic images, ranked 7th in the "ISIC2017: Skin Lesion Analysis toward Melanoma Detection - Part1: Segmentation". Full description of the segmentation method is available in the above-mentioned paper**

mDRFI is the modified version of the DRFI model for saliency detection described in the paper "the paper Salient Object Detection: A Discriminative Regional Feature Integration Approach" (arXiv: https://arxiv.org/pdf/1410.5926.pdf).

We have added some new regional property descriptors to the saliency features in order to better detect the lesions in dermoscopic image. Also, a new pseudo background region is proposed to elevate the saliency detection.

This implementation contains the full pipiline of the saliency detection approach (mDRFI), including both the training and testing phases. Colour constancy correction is also implemented in the codes.

First of all, run the compile.m to compile the mex files (You need c++ compiler, like Microsoft Visual Studio on windows, to be able to do that). If you want to train your own Random Forest regressor, check the trainAll.m for instructions. For more details on features' descriptions, check out our technical report https://arxiv.org/abs/1703.00087.

Tested on Windows 7 64bit with MATLAB 2014b and Ubuntu 14.04 64bit with MATLAB 2015a.

Bugs, comments are welcome to m.jahanifar@modares.ac.ir.
