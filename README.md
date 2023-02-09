# OpenDR datasets

This repository contains datasets collected and annotated within the scopes of the [OpenDR](https://github.com/opendr-eu/opendr) project. The datasets are read in `opendr` format, but they can also be downloaded in their raw format and used in any tool. 

## Installation and requirements

The OpenDR toolkit is an _optional_ requirement of this package, only needed if you plan to use these datasets with an OpenDR tool. For full integration, the [OpenDR](https://github.com/opendr-eu/opendr) toolkit must be installed first.

```
pip install git+https://github.com/opendr-eu/datasets.git
```

If you don't plan on using other OpenDR tools, the datasets can be downloaded from their corresponding README pages, and there is no need to install this package. 


## List of datasets

### Object Detection 2D

- [AGI Humans in Fields dataset](examples/agi_humans)

### Synthetic Datasets
- [Multi-view Facial Image Dataset Based on LFW](https://zenodo.org/record/5809158#.Y-JcIHZByUk)
- [Multi-view Facial Image Dataset Based on CelebA](https://zenodo.org/record/5809273#.Y-JdZXZByUk)
- [AUTH-OpenDR Mixed Image Annotated Dataset for Human-centric Perception Tasks](https://zenodo.org/record/5801594#.Y-TgqhxBxhE)
Description: The dataset was generated through a mixed (real and synthetic) image data generation method which utilizes real background images and DL-generated human models. It contains 50000 real images depicting urban scenes, populated by synthetic human models in various positions and poses and   is suitable for training/evaluating (a) pose estimation, (b) person detection, (c) identity recognition methods. Annotations for 2D bounding boxes of the depicted humans, their  IDs and 2D keypoints etc are provided. The 133 3D human models, required by the method, were generated using the Pixel-aligned Implicit Function (PIFu) and full-body images of people from the Clothing Co-Parsing (CCP) dataset. As background images, a subset of the Cityscapes dataset was used. The Cityscapes license prohibits the distribution of any modified versions of itself. Thus, we provide code  that can re-generate the exact same dataset, given that the Cityscapes dataset is downloaded by the website of its authors.

Code and instructions for re-generating the dataset are provided [here](https://github.com/opendr-eu/opendr/tree/master/projects/python/simulation/human_dataset_generation).

- [AUTH-OpenDR SMPL+D Human Bodies Dataset](https://zenodo.org/record/5801562#.Y-TgrBxBxhE)

Description: The  dataset contains 2982 human bodies in various shapes and textures folowing the SMPL-D template. At its core, our dataset  consists of 183 unique SMPL+D bodies, which were generated through non-rigid shape registration of manually generated MakeHuman models. The rest were generated by applying shape and texture alterations to those models. In addition, we provide code for converting those human models in the FBX format.  However, pose-dependent deformations are not applied to the human models. Finally, instructions for setting a demo project in the Webots simulator are provided. In the project, one the SMPL+D models in FBX format can perform an animation from AMASS.

The dataset is available through the official GitHub repository of the OpenDR toolkit [here](https://github.com/opendr-eu/opendr/tree/master/projects/python/simulation/SMPL%2BD_human_models).
