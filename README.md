# awesome video object/instance segmentation
A curated list of awesome video object/instance segmentation resources.

*Last updated: 2020/12/17*

## What is video object segmentation and video instance segmentation?

Video object segmentation is a binary labeling problem aiming to separate foreground object(s) from the background region of a video.

Video instance segmentation not only need to segment foreground object(s)/instance(s), but also have to identify the category of each object and keep tracking objects across frames.


## Dataset
- DAVIS [`[Download]`](https://davischallenge.org/davis2017/code.html#semisupervised)
- YouTube-VOS and -VIS [`[Download]`](https://youtube-vos.org/dataset/vis/)


## Table of Contents
- [Video object segmentation](#video-object-segmentation)
- [Video instance segmentation](#video-instance-segmentation)


## Video object segmentation
- A Benchmark Dataset and Evaluation Methodology for Video Object Segmentation | **[CVPR' 16]** |[`[pdf]`](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Perazzi_A_Benchmark_Dataset_CVPR_2016_paper.pdf)
- (**OSVOS**) One-Shot Video Object Segmentation | **[CVPR' 17]** |[`[pdf]`](https://openaccess.thecvf.com/content_cvpr_2017/papers/Caelles_One-Shot_Video_Object_CVPR_2017_paper.pdf) | [`[code]`](https://github.com/kmaninis/OSVOS-PyTorch)
- (**MaskTrack**) Learning Video Object Segmentation from Static Images | **[CVPR' 17]** |[`[pdf]`](https://openaccess.thecvf.com/content_cvpr_2017/papers/Perazzi_Learning_Video_Object_CVPR_2017_paper.pdf) | [`[code]`](https://github.com/omkar13/masktrack)
- (**OSVOS-S**) Video object segmentation without temporal information | **[TPAMI' 18]** |[`[pdf]`](https://arxiv.org/pdf/1709.06031.pdf)
- (**Lucid**) Lucid Data Dreaming for Video Object Segmentation | **[IJCV' 19]** |[`[pdf]`](https://link.springer.com/article/10.1007/s11263-019-01164-6) | [`[code]`](https://github.com/yelantf/pyLucid)
- (**RANet**) RANet: Ranking Attention Network for Fast Video Object Segmentation | **[ICCV' 19]** |[`[pdf]`](https://arxiv.org/pdf/1908.06647.pdf) | [`[code]`](https://github.com/Storife/RANet)
- (**e-OSVOS**) Make One-Shot Video Object Segmentation Efficient Again | **[NIPS' 20]** |[`[pdf]`](https://proceedings.neurips.cc//paper/2020/file/781397bc0630d47ab531ea850bddcf63-Paper.pdf) | [`[code]`](https://github.com/dvl-tum/e-osvos)



## Video instance segmentation


## Performance

### DAVIS16 VAL
| Method                |year  |Technique| J      | F      | J&F   |TIME(MS)|
| :----:                |:----:|  :----: | :----: | :----: | :----:| :----: |
| OSVOS                 |2017  | OL      | 79.8   | 80.6   |80.2   | 10000  |
| MaskTrack             |2017  | OL+OF   | 79.7   | 75.4   |77.6   | 12000  |
| OSVOS-S               |2018  | OL      | 85.6   | 87.5   |86.6   |        |
| Lucid                 |2019  | OL+OF   | 83.9   | 82.0   |83.0   |        |
| RANet                 |2019  |         | 85.5   | 85.4   |85.5   | 33     |
| RANet                 |2019  | OL      | 86.6   | 87.6   |87.1   | 4000   |
| e-OSVOS               |2020  | OL      | 86.6   | 87.0   |86.8   | 3450   |



### DAVIS17 VAL
| Method                |year  |Technique| J      | F      | J&F   |TIME(MS)|
| :----:                |:----:|  :----: | :----: | :----: | :----:| :----: |
| OSVOS                 |2017  | OL      | 56.6   |63.9    | 60.3  | 10000  |
| OSVOS-S               |2018  | OL      | 64.7   |71.3    | 68.0  |        |
| RANet                 |2019  |         | 63.2   |68.2    | 65.7  | 33     |
| e-OSVOS               |2020  | OL      | 74.4   |80.0    | 77.2  | 3450   |



### DAVIS17 TEST
| Method                |year  |Technique| J      | F      | J&F   |TIME(MS)|
| :----:                |:----:|  :----: | :----: | :----: | :----:| :----: |
| OSVOS                 |2017  | OL      |47.0    | 54.8   |50.9   | 10000  |
| OSVOS-S               |2018  | OL      |52.9    | 62.1   |57.5   |        |
| Lucid                 |2019  | OL+OF   |63.4    | 69.9   |66.6   |        |
| RANet                 |2019  |         |53.4    | 57.3   |55.4   | 33     |
| e-OSVOS               |2020  | OL      |60.9    | 68.6   |64.8   | 3450   |



### YouTube-VOS VAL
| Method                |year  |Technique| Overall|TIME(MS)|
| :----:                |:----:|  :----: | :----: | :----: |
| OSVOS                 |2017  | OL      | 58.8   | 10000  |
| e-OSVOS               |2020  | OL      | 71.4   | 3450   |



### YouTube-VIS
| Method                | Optical Flow | VAL AP |TEST AP|  FPS        |
| :----:                |      :----:  | :----: |:----: | :----:      |
| MaskTrack R-CNN       |      ✘       | 30.3   |32.3   |20 (1080Ti)  |




## Contact & Feedback
If you have any suggestions about papers, feel free to mail me :)
- [e-mail](mailto:bomiaobbb@gmail.com)
- [pull request](https://github.com/bo-miao/awsome-video-object-instance-segmentation/pulls)