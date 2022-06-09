# CoSOD3K (CVPR2020) <a name="headin"></a>

'Taking a Deeper Look at Co-Salient Object Detection'

### Table of Contents
- [CoSOD3K (CVPR2020) <a name="headin"></a>](#cosod3k-cvpr2020-)
	- [Table of Contents](#table-of-contents)
	- [Abstract](#abstract)
	- [CoSOD Dataset Comparision](#cosod-dataset-comparision)
	- [Statistics of DAVSOD](#statistics-of-davsod)
	- [Downloads](#downloads)
	- [Usage](#usage)
	- [Results](#results)
	- [Citation](#citation)
## Abstract
Co-salient object detection (CoSOD) is a newly emerging and rapidly growing branch of salient object detection (SOD), which aims to detect the co-occurring salient objects in multiple images. However, existing CoSOD datasets often have a serious data bias, which assumes that each group of images contains salient objects of similar visual appearances. This bias results in the ideal settings and the effectiveness of the models, trained on existing datasets, may be impaired in real-life situations, where the similarity is usually semantic or conceptual. To tackle this issue, we first collect a new high-quality dataset, named CoSOD3k, which contains 3,316 images divided in 160 groups with multiple level annotations, i.e., category, bounding box, object, and instance levels. CoSOD3k makes a significant leap in terms of diversity, difficulty and scalability, benefiting related vision tasks. Besides, we comprehensively summarize 34 cutting-edge algorithms, benchmarking 19 of them over four existing CoSOD datasets (MSRC, iCoSeg, Image Pair and CoSal2015) and our CoSOD3k with a total of ∼61K images (largest scale), and reporting group-level performance analysis. Finally, we discuss the challenge and future work of CoSOD. Our study would give a strong boost to growth in the CoSOD community.

## CoSOD Dataset Comparision

## Citation
If you find this useful, please cite the following work:

```
@inproceedings{fan2020taking,   
  title={Taking a Deeper Look at the Co-salient Object Detection}, 
  author={Fan, Deng-Ping and Lin, Zheng and Ji, Ge-Peng and Zhang, Dingwen and Fu, Huazhu and Cheng, Ming-Ming},   
  booktitle={IEEE CVPR}, 
  year={2020} 
} 
