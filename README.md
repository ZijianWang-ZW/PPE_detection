# Real-time PPE Detection & Open Dataset

![avatar](figures/ppe_sample.gif)

## Introduction

The repository introduces eight DL models built on You Look Only Once (YOLO) architecture for PPE detection. Meanwhile, a novel high-quality dataset is constructed for detecting the person, the vest, and four helmet colors.

## Framework

![avatar](figures/methodology.PNG)

## CHV Dataset

A novel dataset  is constructed for detecting the helmet, the helmet colors and the person for this project, named **Color Helmet and Vest (CHV)** dataset. 

Instead of just accepting exiting images, strict criteria are designed at the beginning, and only  1,330 high-quality images among 10,000 ones from the Internet and open datasets are selected. 

<div align=center><img src="figures/size_class.png" width="60%" /></div>



The dataset is open for free use, please download at [Google Drive](https://drive.google.com/file/d/1fdGn67W0B7ShpBDbbQpUF0ScPQa4DR0a/view?usp=sharing) or [Baidu Yunpan (password: f003)](https://pan.baidu.com/s/1G9EbLKUgF1tcOPCeWSEeMw ). 

If the dataset helpes you, please cite the repository in your article:

`@misc{Zijian2020,
	author = {Zijian Wang}, title = {PPE detection}, year = {2020},
	publisher = {GitHub}, journal = {GitHub repository},
	howpublished = {\url{https://github.com/ZijianWang1995/PPE_detection}}}`

## Results

- **YOLO v5x owns the best mAP, 86.55%.**
- **YOLO v5s has the faster processing speed, 52 FPS.**
- For YOLO v3 models, different detection layers are tested, while the more layers cannot improve the performance. 
- For YOLO v4 models,  the increase of training image size cannot contribute to better performance. 

<center><img src="figures/map.png" style="zoom:100%;"/> 

<center>Figure: Mean average precision in each model. </center>

<div align=center><img src="figures/time.png" width="60%"/></div>

<center>Figure: Average time for processing one image in each model (GPU: Tesla P40 with 24 GB; CPU: 4 cores with 8 GB)  </center>

 ## Todo 

- Add the weights, and how to train the model

