# CoSOD3K (CVPR2020) <a name="headin"></a>

'Taking a Deeper Look at Co-Salient Object Detection'

### Table of Contents
- [CoSOD3K (CVPR2020) <a name="headin"></a>](#cosod3k-cvpr2020-)
	- [Table of Contents](#table-of-contents)
	- [Abstract](#abstract)
	- [CoSOD Dataset Comparision](#cosod-dataset-comparision)
	- [Statistics](#statistics)
	- [Downloads](#downloads)
	- [SOTA Models](#sota-models)
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

## SOTA Models

#### News

|      Model       |  Pub.   | Year |      #Training       |           Training set            |               Main Component               | SL.  | Sp.  | Po.  | Ed.  | Post. |
| :--------------: | :-----: | :--: | :------------------: | :-------------------------------: | :----------------------------------------: | :--: | :--: | :--: | :--: | :---: |
| WPL<sup>T</sup>  |  UIST   | 2010 |                      |                                   |   Morphological, Translational Alignment   |  U   |      |      |      |       |
| PCSD<sup>T</sup> |  ICIP   | 2010 |       120,000        |          8*8 image patch          |        Sparse feature, Filter Bank         |  W   |      |      |      |       |
| IPCS<sup>T</sup> |   TIP   | 2011 |                      |                                   |         Ncut, co-multilayer Graph          |  U   |  √   |      |      |       |
| CBCS<sup>T</sup> |   TIP   | 2013 |                      |                                   |     Contrast/Spatial/Corresponding Cue     |  U   |      |      |      |       |
|  MI<sup>T</sup>  |   TMM   | 2013 |                      |                                   | Feature/Images Pyramid, Multi-scale Voting |  U   |  √   |      |      | GCut  |
| CSHS<sup>T</sup> |   SPL   | 2013 |                      |                                   |   Hierarchical Segmentation, Contour Map   |  U   |      |      |  √   |       |
| ESMG<sup>T</sup> |   SPL   | 2014 |                      |                                   |   Efficient Manifold Ranking 184\], OTSU   |  U   |      |      |      |       |
|  BR<sup>T</sup>  |   MM    | 2014 |                      |                                   |  Common/Center Cue, Global Correspondence  |  U   |  √   |      |      |       |
| SACS<sup>T</sup> |   TIP   | 2014 |                      |                                   |   Self-adaptive Weight, Low Rank Matrix    |  U   |  √   |      |      |       |
|       DIM        |  TNNLS  | 2015 |     1,000+9,963      |              ASD+PV               |     SDAE model, Contrast/Object Prior      |  S   |  √   |      |      |       |
|       CODW       |  IJCV   | 2016 |                      |        ImageNet pre-train         |        SermaNet, RBM, IMC, IGS, IGC        |  W   |  √   |  √   |      |       |
|      SP-MIL      |  TPAMI  | 2017 |    (240+643)•10%     |          MSRC-V1+iCoseg           |       SPL 1971, SVM, GIST 1691, CNNs       |  W   |  √   |      |      |       |
|        GD        |  IJCAI  | 2017 |        9,213         |              MSCOCO               |     VGGNet16 \[681, Group-wise Feature     |  S   |      |      |      |       |
|      MVSRCC      |   TIP   | 2017 |                      |                                   |    LBP, SIFT \[611, CH, Bipartite Graph    |      |  √   |  √   |      |       |
|       UMLF       |  TCSVT  | 2017 |    (240+2015)*50%    |        MSRC-V1 + CoSa12015        |       SVM, OMR 186\], metric teaming       |  S   |  √   |      |      |       |
|       DML        |  BMVC   | 2018 | 10,000+6,232+ 5,168  |      MIOK+THUR-15K 1111 +DO       |            CAE, HSR, Multistage            |  S   |      |      |      |       |
|       DWSI       |  AAAI   | 2018 |                      |                                   |    EdgeBox \[106\], Low-rank Matrix, CH    |  S   |      |  √   |      |       |
|      GONet       |  ECCV   | 2018 |                      |        ImageNet pre-train         |  ResNet-50 \[281, Graphical Optimization   |  W   |  √   |      |      |  CRF  |
|       COC        |  IJCAI  | 2018 |                      |        ImageNet pre-train         |     ResNet-50 \[281, Co-attention Loss     |  W   |      |  √   |      |  CRF  |
|       FASS       |   MM    | 2018 |                      |        ImageNet pre-train         |    DHS 156\]/VGGNet. Graph optimization    |  W   |  √   |      |      |       |
| PJO<sup>T</sup>  |   TIP   | 2018 |                      |                                   |         Energy Minimization, BoWs          |  U   |  √   |      |      |       |
|       SPIG       |   TIP   | 2018 | 10,000+210+2,015+240 |    MIOK+IPCS+CoSal2015+ MSRC-V    |       DeepLab, Graph Representation        |  S   |  √   |      |      |       |
|       QGF        |   TMM   | 2018 |                      |        ImageNet pre-traln         |   Dense Correspondence, Quality Measure    |  S   |  √   |      |      |  THR  |
|       EHL        |   NC    | 2019 |         643          |              iCoseg               |               GoogLeNet, FSM               |  S   |  √   |      |      |       |
|       IML        |   NC    | 2019 |         3624         |          CoSa12015+PV+CR          |                  VGGNet16                  |  S   |  √   |      |      |       |
|       DGFC       |   TIP   | 2019 |      \>200,000       |            MSCOCO 1551            |        VGGNet16, Group-wise Feature        |  S   |  √   |      |      |       |
|      RCANet      |  IJCAI  | 2019 |      \>200,000       | MSCOCO+COS+iCoseg+ CoSa12015+MSRC |         VGGNet16, Recurrent Units          |  S   |      |      |      |  THR  |
|        GS        |  AAAI   | 2019 |       200,000        |             COCO-SEG              |    VGGNet19, Co-category Classification    |  S   |      |      |      |       |
|      MGCNet      |  ICME   | 2019 |                      |                                   |        Graph Convolutional Networks        |  S   |  √   |      |      |       |
|      MGLCN       |   MM    | 2019 |         N/A          |                N/A                |   VGGNet16, PiCANet, Inter-/Intra-graph    |  S   |  √   |      |      |       |
|        HC        |   MM    | 2019 |         N/A          |                N/A                |     VAE-Net, Hierarchical Consistency      |  S   |  √   |  √   |      |  CRF  |
|       CSMG       |  CVPR   | 2019 |        25,00         |                MB                 |    VGGNet16, Shared Superpixel Feature     |  S   |  √   |      |      |       |
|     DeepCO3      |  CVPR   | 2019 |        10,000        |               MIOK                |      SVFSaI / VGGNet, Co-peak Search       |  W   |      |  √   |      |       |
|       GWD        |  ICCV   | 2019 |      \>200,000       |              MSCOCO               |      VGGNet19 , RNN, Group-wise Loss       |  S   |      |      |      |  THR  |
|      GCAGC       |  CVPR   | 2020 |      \>200,000       |             COCO-SEG              |                Graph Model                 |  S   |      |      |      |       |
|       GICD       |  ECCV   | 2020 |        8,250         |            DUTS\_class            |                  Gradient                  |  S   |      |      |      |       |
|      ICNet       | NeurIPS | 2020 |        9,213         |              COCO-9k              |             External SOD Model             |  S   |      |      |      |       |
|     CoADNet      | NeurIPS | 2020 |      \>200,000       |       DUTS\_class+COCO-SEG        |                Group Mining                |  S   |      |      |      |       |
|    CoSformer     |  arXiv  | 2021 |      \>200,000       |       DUTS\_class+COCO-SEG        |                Transformer                 |  S   |      |      |      |       |
|     CoEG-Net     |  TPAMI  | 2021 |        8,250         |            DUTS\_class            |                    PCA                     |  S   |      |      |      |       |
|     DeepACG      |  CVPR   | 2021 |      \>200,000       |             COCO-SEG              |        Gromov-Wasserstein Distance         |  S   |      |      |      |       |
|      GCoNet      |  CVPR   | 2021 |        8,250         |            DUTS\_class            |        Group Collaborative Learning        |  S   |      |      |      |       |
|       CADC       |  ICCV   | 2021 |     8,250+9,213      |        DUTS\_class+COCO-9k        |            Dynamic Convolution             |  S   |      |      |      |       |
|       DCFM       |  CVPR   | 2022 |        9,213         |              COCO-9k              |    Prototype, self-contrastive learning    |  S   |      |      |      |       |
|       UFO        |  arXiv  | 2022 |      \>200,000       |             COCO-SEG              |                Transformer                 |  S   |      |      |      |       |
|     GCoNet+      |  arXiv  | 2022 |      \>200,000       |  DUTS\_class, COCO-9k, COCO-SEG   |   Inter-group Learning, Metric Learning    |  S   |      |      |      |       |

> WPL<sup>T</sup> means the WPL is a traditional method, instead of a deep method.

## Results

#### SOTA:

Refer to the [CoSOD task in papers-with-code](https://paperswithcode.com/task/co-saliency-detection).

#### Predicted Maps

|  Model   |                          Baidu Pan                           |                         Google Drive                         |
| :------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|   CBCS   | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1nfwmzj9UuYGyFVijT6Uwzg) (gtse) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/19gPOFNYXvTmSqWnLeOtq9rkDyB8dXXMl/view?usp=sharing) |
|   CODR   | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1Cs6Q4YAlG2IVzAaQhi_Oew) (qfks) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1gPm17eGISZ0EA8_HkCPQk6horeUwwNeQ/view?usp=sharing) |
|   CPD    | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1ViUFlkr6MT_98eSYhJkRQg) (jxkk) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/145FCYr2RVpQ7xOHZNhVa-J81G6FoqhXD/view?usp=sharing) |
|   CSHS   | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1jDHk1rYdzj6cZVdRilxowg) (wda4) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1BRWNFboc9AhChQq5NnA-y11xVTiEFtaR/view?usp=sharing) |
|   CSMG   | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1BGoIOrWutFeU4EXtqsgG6Q) (gwm6) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1fgeCS2JEskuRSuZkJHOq2xxi1haZFYFa/view?usp=sharing) |
|   DIM    | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1KDK2hMP4v2QIifqYZ2zRqg) (2hgk) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1yY_De6Nbip4lzRMxXhU5LNh-K036BRJ7/view?usp=sharing) |
|  EGNet   | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/16jSIRvSUPL14qIc2DMqyQA) (tkna) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1D1XSpR3y-139Gvy_YaWKfxFZaHeA9ryv/view?usp=sharing) |
|   ESMG   | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1q4BsnDeYsrFVHrE8GdnZbQ) (hxqb) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1yEdgTzVHtbUOESHzdxDqIZ6OM2F2uw1l/view?usp=sharing) |
|   IML    | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1OYrdSLNBEuUzJRqsw-Pc5g) (7m1c) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1CvW8roAkBXTM62DzSq03AyzaGSMW2N56/view?usp=sharing) |
|   UMLF   | [Baidu-Disk](https://web.archive.org/web/20220125070207/https://pan.baidu.com/s/1aNvZ0CiI3cj0VpSDrIGVQw) (eqpw) | [Google-Drive](https://web.archive.org/web/20220125070207/https://drive.google.com/file/d/1tNwd_EFN-bMrclwCMOZYJHxAI-MkXMH8/view?usp=sharing) |
|  GCAGC   | [Baidu-Disk](https://pan.baidu.com/s/1xFPn2PiWT3wgR6OEHhlczg) (ij29) | [Google-Drive](https://drive.google.com/drive/folders/1EOnukW5iRbTe3liblrl0IGavzI8mXJz5?usp=sharing) |
|   GICD   | [Baidu-Disk](https://pan.baidu.com/s/1P35BdU8EFJX9JK9tEGTa1Q) (puji) | [Google-Drive](https://drive.google.com/drive/folders/1FDwIn2IS_E23mbcuBbezg-9-pUg92EGY?usp=sharing) |
|  ICNet   | [Baidu-Disk](https://pan.baidu.com/s/1WFQxeIOjOiByiFYHLpuytA) (xwcv) | [Google-Drive](https://drive.google.com/file/d/1px4tPVWAgbBPMt6Rp23oNwWz8Ulj6pmX/view?usp=sharing) |
| CoADNet  | [Baidu-Disk](https://pan.baidu.com/s/1A9TFQ6yC73ulR6UmJ4QMCw) (MVPL) |                                                              |
| Co-EGNet | [Baidu-Disk](https://pan.baidu.com/s/19hIlViLbby-a7vQw17ZTVw) (f4p3) | [Google-Drive](https://drive.google.com/file/d/1AK9UNR5mLHQakOTkRawcKSDg8YwIu-xJ/view?usp=sharing) |
|  GCoNet  |                                                              | [Google-Drive](https://drive.google.com/file/d/17LgbcwGNK1DFl9jRAoMxF2796YlQYR4a/view?usp=sharing) |
|   CADC   | [Baidu-Disk](https://pan.baidu.com/s/1bkCrqsOzNAgH-VSM0p7fMA) (i59u) | [Google-Drive](https://drive.google.com/file/d/1LBBQOBeasn6O2caccs5t1e26ilv-d62h/view?usp=sharing) |
|   DCFM   |                                                              | [Google-Drive](https://drive.google.com/file/d/1wGeNHXFWVSyqvmL4NIUmEFdlHDovEtQR/view?usp=sharing) |
|   UFO    |                                                              | [Google-Drive](https://drive.google.com/drive/folders/1QCr0zCCIsBC7JEHBS6A1O3V2JIpEAHyr?usp=sharing) |
| GCoNet+  |                                                              | [Google-Drive](https://drive.google.com/drive/folders/1QpqHJKzj1aFddqNHb6bDbVOXTWlowb14?usp=sharing) |

#### Qualitative Results

<p align="center">
    <img src="figures/Co-SOD3K-Results.png" width="100%"/> <br/>
    <em> 
    Figure 3: Qualitative examples of existing top-10 models on CoSOD3k.
    </em>
</p>



## Citation
If you find this useful, please cite the following work:

```
@inproceedings{fan2020taking,   
  title={Taking a Deeper Look at the Co-salient Object Detection}, 
  author={Fan, Deng-Ping and Lin, Zheng and Ji, Ge-Peng and Zhang, Dingwen and Fu, Huazhu and Cheng, Ming-Ming},   
  booktitle={IEEE CVPR}, 
  year={2020} 
} 
