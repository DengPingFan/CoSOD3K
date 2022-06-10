# CoSOD3K (CVPR2020) <a name="headin"></a>

'Taking a Deeper Look at Co-Salient Object Detection'

### Table of Contents
- [CoSOD3K (CVPR2020) <a name="headin"></a>](#cosod3k-cvpr2020-)
	- [Table of Contents](#table-of-contents)
	- [Abstract](#abstract)
	- [CoSOD Dataset Comparision](#cosod-dataset-comparision)
	- [Statistics](#statistics)
	- [Downloads](#downloads)
	- [Usage](#usage)
	- [Results](#results)
	- [Citation](#citation)
## Abstract
Co-salient object detection (CoSOD) is a newly emerging and rapidly growing branch of salient object detection (SOD), which aims to detect the co-occurring salient objects in multiple images. However, existing CoSOD datasets often have a serious data bias, which assumes that each group of images contains salient objects of similar visual appearances. This bias results in the ideal settings and the effectiveness of the models, trained on existing datasets, may be impaired in real-life situations, where the similarity is usually semantic or conceptual. To tackle this issue, we first collect a new high-quality dataset, named CoSOD3k, which contains 3,316 images divided in 160 groups with multiple level annotations, i.e., category, bounding box, object, and instance levels. CoSOD3k makes a significant leap in terms of diversity, difficulty and scalability, benefiting related vision tasks. Besides, we comprehensively summarize 34 cutting-edge algorithms, benchmarking 19 of them over four existing CoSOD datasets (MSRC, iCoSeg, Image Pair and CoSal2015) and our CoSOD3k with a total of ∼61K images (largest scale), and reporting group-level performance analysis. Finally, we discuss the challenge and future work of CoSOD. Our study would give a strong boost to growth in the CoSOD community.

## CoSOD Dataset Comparision
<p align="center">
    <img src="figures/CoSOD3K.png" width="100%"/> <br/>
    <em> 
    Figure 1: Different salient object detection (SOD) tasks. (a) Traditional SOD [78]. (b) Within image co-salient object detection (CoSOD) [93], where common salient objects are detected from a single image. (c) Existing CoSOD, where salient objects are detected according to a pair [52] or a group [85] of images with similar appearances. (d) The proposed CoSOD in the wild, which requires a large amount of semantic context, making it more challenging than existing CoSOD.
    </em>
</p>

<p align="center">
    <img src="figures/CoSOD3k2.png" width="100%"/> <br/>
    <em> 
    Figure 2: The 160 Objects from our CoSOD3k.
    </em>
</p>

## Statistics
<p align="center">
    <img src="figures/CoSOD3k-statistic.png" width="60%"/> <br/>
    <em> 
    Table 1: Statistics for size and number of instances/objects in existing datasets.’-’ indicates that the dataset only contains object-level annotations, so, the number of instances is only one.
    </em>
</p>

## Downloads
|**Year**|**Publisher**|**Paper**|**#Image**|**Download Link1**|**Download Link2**|
| :-: | :-: | :-: |  :-: | :-: | :-: |
|2005|ICCV|**MSRC**|233|[Baidu Pan: 8r27](https://pan.baidu.com/s/1IiHNfQuLl4jJVmxu3okKFw)|[Google (4.17M)](https://drive.google.com/file/d/1Tnb31AavpDpNiTDyJmp-ucx21HC_ieOS/view?usp=sharing)|
|2010|CVPR|**iCoSeg**|643|[Baidu Pan: e1mz](https://pan.baidu.com/s/11VlWTeZTZVnj_H3InWhBaw)|[Google (67M)](https://drive.google.com/file/d/1WBWd-Me1mliLgErLsv6MDxPzvU510jQd/view?usp=sharing)|
|2011|TIP|**Image Pair**|105|[Baidu Pan: fmqj](https://pan.baidu.com/s/1Hs3gSbor3ZWLafVhK3MWJw)|[Google (0.98M)](https://drive.google.com/file/d/1NC96TcxmAM8ntgFK0iXUbcgDko3uI6qu/view?usp=sharing)|
|2016|IJCV/CVPR|**CoSal2015**|2015|[Baidu Pan: kpvv](https://pan.baidu.com/s/1DR5wKiew0H3t7ZlYHrCgnw)|[Google (96.1M)](https://drive.google.com/file/d/1mmYpGx17t8WocdPcw2WKeuFpz6VHoZ6K/view?usp=sharing)|
|2018|AAAI|**WICOS**|364|[Baidu Pan: b5qg](https://pan.baidu.com/s/1R41b9S0pGGdBiy6IABrEIQ)|[Google (10.7M)](https://drive.google.com/file/d/1Nfr9fLV7N1Obj9cQERvk1pqp4R1CJp8k/view?usp=sharing)|
|2020|ECCV|**CoCA**|1295|[Baidu Pan: ckzt](https://pan.baidu.com/s/1pgLzxf0jCns3hFDJZ6PkbQ)|[Google (96M)](https://drive.google.com/file/d/1mnVUbag9Yz_m0pBg_IBIBjlAhFGenatR/view?usp=sharing)|
|2020|CVPR|**CoSOD3k**|3316|[Baidu Pan: 65as](https://pan.baidu.com/s/1xXmgY4OgMi50zZmndS8cYA)|[Google (418M)](https://drive.google.com/file/d/1-zkz9Zu3vvT7JB_n7jTZYiTxBpoigER6/view?usp=sharing) + [Google (411M)](https://drive.google.com/file/d/1TKGZOn4oxmoaQYHzb8ynpQ_5pEFrPaZG/view?usp=sharing)|
|Overall | | |  |[Baidu Pan: 6mvn](https://pan.baidu.com/s/1CJ1DTjMl6D9XvS618sKJ_g)|[Google (1.4G)](https://drive.google.com/drive/folders/1OdD4yCoMJHmBhJR90OUT8MkBt-LJggHV?usp=sharing)|

## Citation
If you find this useful, please cite the following work:

```
@inproceedings{fan2020taking,   
  title={Taking a Deeper Look at the Co-salient Object Detection}, 
  author={Fan, Deng-Ping and Lin, Zheng and Ji, Ge-Peng and Zhang, Dingwen and Fu, Huazhu and Cheng, Ming-Ming},   
  booktitle={IEEE CVPR}, 
  year={2020} 
} 
