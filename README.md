# AffectNet-D and RaFD-D

AffectNet-D and RaFD-D are datasets that contain depthmaps for a subset of AffectNet (~87K) and RaFD (~4K) images. 
AffectNet is a large-scale in-the-wild face dataset that consists of 8 different expressions as well as valence and arousal annotations. 
Similarly, RaFD provides a dataset that contains facial expression in a controlled environment.

## Details

We propose to augment existing expression annotated datasets, AffectNet and RaFD, with depth information. To this end, we propose to use an existing state-ofthe-art method to reconstruct the 3D models of faces. We carefully investigated the quality of the reconstructed 3D models and discarded the ones which are not fitted well. From these 3D models, we computed the corresponding depth maps and surface normal maps. 

![Pipeline](https://github.com/rumi-b/3d-dense_geo_expression_synthesis/blob/main/images/depthmap_pipeline.png)

| Dataset     | Anger | Contempt | Disgust | Fear | Happy | Neutral | Sadness | Surprise | Total |
| ------------|:-----:|:--------:|:-------:|:----:|:-----:|:-------:|:-------:|:--------:|:-----:|
| AffectNet-D | 15,000|3,703     |3,726    |6,073 |15,000 |15,000   |15,000   |13,604    |87,106 |
| RaFD-D      | 564   |580       |576      | 548  | 557   |585      |569      | 515      |4,494  |

## Samples


<img src="https://github.com/rumi-b/3d-dense_geo_expression_synthesis/blob/main/images/depth_samples.png" width="900" height="750">

## Downloads
Link to download [AffectNet-D](https://drive.google.com/file/d/1i89A_br_OA2Oe5fjrwaOvpzo-Fw4ClSe/view?usp=sharing)

Link to download [RaFD-D](https://drive.google.com/file/d/1Z5WL2bUZw5w9SjoIHo2Se3mdn19AU7Xt/view?usp=sharing)


## Agreement

The AffectNet-D and RaFD-D datasets are available for non-commercial research purposes only.
All images of the AffectNet dataset are obtained from the Internet by. 
You agree not to reproduce, duplicate, copy, sell, trade, resell or exploit for any commercial purposes, any portion of the images and any portion of derived data. The publishers reserve the right to terminate your access to the datasets at any time.

## Citation
```
@InProceedings{Bodur_2021_WACV,
    author    = {Bodur, Rumeysa and Bhattarai, Binod and Kim, Tae-Kyun},
    title     = {3D Dense Geometry-Guided Facial Expression Synthesis by Adversarial Learning},
    booktitle = {Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)},
    month     = {January},
    year      = {2021},
    pages     = {2392-2401}
}
```
