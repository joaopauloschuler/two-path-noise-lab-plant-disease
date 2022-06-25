[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/reliable-deep-learning-plant-leaf-disease/image-classification-on-plantvillage)](https://paperswithcode.com/sota/image-classification-on-plantvillage?p=reliable-deep-learning-plant-leaf-disease)

# Reliable Deep Learning Plant Leaf Disease Classification Based on Light-Chroma Separated Branches
This repository contains the source code for the paper [Reliable Deep Learning Plant Leaf Disease Classification Based on Light-Chroma Separated Branches](https://www.researchgate.net/publication/355215213_Reliable_Deep_Learning_Plant_Leaf_Disease_Classification_Based_on_Light-Chroma_Separated_Branches) by Joao Paulo Schwarz Schuler, Santiago Romani, Mohamed Abdel-Nasser, Hatem Rashwan and Domenec Puig. The [baseline](https://github.com/joaopauloschuler/two-path-noise-lab-plant-disease/tree/main/raw/baseline) folder contains the source code used to train our baseline model while the [two-paths](https://github.com/joaopauloschuler/two-path-noise-lab-plant-disease/tree/main/raw/two-paths) folder contains our two-paths LAB feed Inception V3 variants.

## Abstract
The Food and Agriculture Organization (FAO) estimated that plant diseases cost the world economy $220 billion in 2019. In this paper, we propose a lightweight Deep Convolutional Neural Network (DCNN) for automatic and reliable plant leaf diseases classification. The proposed method starts by converting input images of plant leaves from RGB to CIE LAB coordinates. Then, L and AB channels go into separate branches along with the first three layers of a modified Inception V3 architecture. This approach saves from 1/3 to 1/2 of the parameters in the separated branches. It also provides better classification reliability when perturbing the original RGB images with several types of noise (salt and pepper, blurring, motion blurring and occlusions). These types of noise simulate common image variability found in the natural environment. We hypothesize that the filters in the AB branch provide better resistance to these types of variability due to their relatively low frequency in the image-space domain.

## Further Reading
You may be interested in our other paper on the same topic and the same dataset [Color-aware two-branch DCNN for efficient plant disease classification](https://github.com/joaopauloschuler/two-branch-plant-disease).

## Citing this Paper 
Bibtex:
```
@inbook{Schuler2021plant,
author = {Schuler, Joao and Romaní, Santiago and Abdel-nasser, Mohamed and Rashwan, Hatem and Puig, Domenec},
year = {2021},
month = {10},
pages = {375-381},
title = {Reliable Deep Learning Plant Leaf Disease Classification Based on Light-Chroma Separated Branches},
booktitle = {Artificial Intelligence Research and Development},
publisher = {IOS Press},
isbn = {9781643682105},
doi = {10.3233/FAIA210157}
}
```
## Running the Code
Due to library updates, the code used for the paper doesn't run on current tensorflow/keras. As of the writting of this readme file, the current version of tensorflow is 2.7. An updated version of the code was done after the paper publication. This version is now compatible with tensorflow 2.7:
* [RGB - Baseline](https://github.com/joaopauloschuler/two-path-noise-lab-plant-disease/blob/main/v2.7/code_example_schuler_baseline_various_mixes_v2_7.ipynb). [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/joaopauloschuler/two-path-noise-lab-plant-disease/blob/main/v2.7/code_example_schuler_baseline_various_mixes_v2_7.ipynb)
* [CIE L* a* b* - Light-Chroma Separated Branches](https://github.com/joaopauloschuler/two-path-noise-lab-plant-disease/blob/main/v2.7/code_example_schuler_two_paths_various_mixes_v2_7.ipynb). [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/joaopauloschuler/two-path-noise-lab-plant-disease/blob/main/v2.7/code_example_schuler_two_paths_various_mixes_v2_7.ipynb)
