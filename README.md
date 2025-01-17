# OpenConstruction

[Ruoxin Xiong](https://www.linkedin.com/in/ruoxin-xiong-56773815b/), [Yuansheng Zhu](https://sites.google.com/view/yuz128/home), [Yanyu Wang](https://www.linkedin.com/in/yanyu-wang-984bb61b7/), [Pengkun Liu](https://www.linkedin.com/in/pengkunliu/), and [Pingbo Tang](https://sites.google.com/site/tangpingbo/)

This is the official implementation of the paper "[Facilitating Construction Scene Understanding Knowledge Sharing and Reuse via Lifelong Site Object Detection](https://link.springer.com/chapter/10.1007/978-3-031-25082-8_15)" in the first [CVCIE workshop](https://vap.aau.dk/cvcie/) at ECCV 2022. 

## Introduction

Automatically recognizing diverse construction resources (e.g., workers and equipment) from construction scenes supports efficient and intelligent workplace management. This work proposed a novel lifelong construction resource detection framework for continuously learning from dynamic changing construction contexts without catastrophically forgetting previous knowledge.

<p align="center">
  <img src="https://user-images.githubusercontent.com/43504654/183323676-1d70bd4c-3282-489c-9239-5d48d8f6df61.png" width=50% height=50%>
</p>

## Demo
![vis.pdf](https://github.com/YUZ128pitt/OpenConstruction/files/9278163/vis.pdf)

## Poster
![poster.pdf](https://github.com/ruoxinx/OpenConstruction/blob/main/documents/ECCV'22%20poster-011.pdf)

## Data preparation and processing

Please download the datasets from their official website under licensed permissions.

### ACID
- Description: 10 categories of construction machines, 10,000 labeled images, 15,767 construction machine objects
- Category: Mobile crane; Tower crane; Concrete mixer truck; Backhoe loader; Wheel loader; Compactor; Dozer; Dump truck; Excavator; Grader
- [Source](https://www.acidb.ca/)

### SODA
- Description: 19,846 images in the dataset and 15 categories of objects
- Category: Person; Helmet; Vest; Board; Wood; Rebar; Brick; Scaffold; Handcart; Cutter; Ebox; Hopper; Hook; Fence; Slogan
- [Source](https://linjiarui.net/en/portfolio/2022-02-22-SODA-site-object-detection-dataset-for-deep-learning-in-construction) 

### MOCS
- Description: 41,668 images in the dataset and 13 categories of objects
- Category: Worker; Tower crane; Hanging hook; Vehicle crane; Roller; Bulldozer; Excavator; Truck; Loader; Pump truck; Concrete transport mixer; Pile driver; Other vehicle
- [Source](http://www.anlab340.com/Archives/IndexArctype/index/t_id/17.html)

## Running environment
This repo is largely based on the [MMDetection2](https://github.com/open-mmlab/mmdetection). Please follow their installation instruction.

## Training and testing
- Step 1: download the config files and put it under the config folder under mmdetection.

- Step 2: modify the file path in the config files.

- Step 3: run `src/run_openconstruction_lifelong.sh` 

- Step 4: enjoy^-^! Please cite our work if you found it helpful and contact us at yz7008@rit.edu if there is any issue.

## Acknowledgments
We sincerely thank [Anlab](http://www.anlab340.com), [AIRCon-Lab](https://profsckang.wixsite.com/uofa-rlab), and [Mechanics Computing and Simulation Laboratory](https://linjiarui.net/en/) for providing the datasets.

## **Citation**

If you find this paper useful in your research, please consider cite:

```
@InProceedings{10.1007/978-3-031-25082-8_15,
author="Xiong, Ruoxin
and Zhu, Yuansheng
and Wang, Yanyu
and Liu, Pengkun
and Tang, Pingbo",
editor="Karlinsky, Leonid
and Michaeli, Tomer
and Nishino, Ko",
title="Facilitating Construction Scene Understanding Knowledge Sharing and Reuse via Lifelong Site Object Detection",
booktitle="Computer Vision -- ECCV 2022 Workshops",
year="2023",
publisher="Springer Nature Switzerland",
address="Cham",
pages="228--243",
isbn="978-3-031-25082-8"
}
```
