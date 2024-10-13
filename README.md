# Papers for Neural Image Compression
**Purpose:** We aim to provide a summary of neural image compression. More papers will be summarized. 

University of Science and Technology of China (USTC), [Intelligent Media Computing Lab](https://faculty.ustc.edu.cn/chenzhibo).

**📌 About new works.** If you want to incorporate your studies (e.g., the link of paper or project) on neural image compression in this repository. Welcome to raise an issue or email us. We will incorporate it into this repository and our survey report as soon as possible.

## Table of contents
- [Survey & Benchmark](#survey--benchmark)
- [Lossless Image Compression](#lossless-image-compression)
- [Near-Lossless Image Compression](#near-lossless-image-compression)
- [Lossy Image Compression](#lossy-image-compression)
  - [Nonlinear Transform Coding](#nonlinear-transform-coding)
    <!-- - [2015](#2015) -->
  - [Generative Image compression](#generative-image-compression)
- [Other tasks](#other-tasks)
<!-- variable rate, adjustable complexity, scalable coding, light field, stereo image and so on  -->
<!--   - [RNN-style](#RNN-style)
  - [VAE-style](#VAE-style)
  - [INR-style](#INR-style)
  - [Invertible transform style](#Invertible-transform-style) -->

## Survey & Benchmark
| Paper | First Author | Venue | 
| :---: | :--: | :--:|
| [Learning-driven lossy image compression: A comprehensive survey](https://pdf.sciencedirectassets.com/craft/capi/cfts/init?s=1800&p=%2F271095%2F1-s2.0-S0952197623X00062%2F1-s2.0-S0952197623005456%2Fmain.pdf&q=X-Amz-Security-Token%3DIQoJb3JpZ2luX2VjEDAaCXVzLWVhc3QtMSJHMEUCIQCzU9L5wxeAKV80LYPeR39i%252FzbHZoIZUIeMCC77kaHX4gIgE90FyXF%252F6mhPJRBJ3s3sGDezW0tafHKCsJdg0O7VGf0qsgUIWRAFGgwwNTkwMDM1NDY4NjUiDNxs9Kz0fLxBcImx8iqPBWoRr7ZWE%252FK%252FrjZpGWiYCmE9fOhDr8hENnhiuT3M3UfjJLjeU224%252BtfmfYmjqVjYNUXLohyUgpdjSIWA1DpPWB8jSc2WoHG36lr1cqtrgG2oMP1keYi6aih0PztvH3uB2LOBlVM5lesO9fuFcQb7ZE0hmq84xgI%252F%252Bhpa%252BanrKZ%252BZXRkmM8aMq1pl%252F45JwU%252BwzmbI3hgaB3hiCiZRkM3vGMRXGCsQcPaukGvT7cHyaJKAkJXs4bGrHYBSv3SLGL0sAXgH0i4roP51sQdnv7hfpfkI90hUlCJA%252Br2U%252BWCyknyei8oVVufPtbe4FqCXu3y0Wl%252B5XsuuClyKeqHACQth6nZC0eJC73wrQjog7p3JcIeQdOiGF%252FjKF3kG4FzNVcMb5TN%252FIHp5MN1bNsWBGaGC3mMQ4E8Vbf6lbn7sn5QFzhnAPW9sKzLFB2jezK4yflNozoI%252FGFJF9MvQSOGeuL0soEMjm4mga6L86WevjekCct9OTVdDiifC2qBLZs8jxUtUzTPVqxBep6uTsYAFAiX76FR505PIg0HvtdsCPomOvzO0wBx6mjpiRBJFij4HaR9Z4B4kRr7Rh3ULpQmxzfI062bahByCkcNra1zmusxPITXzcvF%252FqJhVSMsbOz%252FTeX0jG%252FQleRcj6AByMKo3RZxgrnPubWkBCkNhPkEyzzqGj0U1ZtC6BtQ494Q5eA7HvfiYLiAS01WUrpWle8VlxACI3UC7v9n%252By0WZftyIc7dxm2sYv3OjaSln13UoGze8dNsJuOEQ5QLfY%252BKavezOkNFhc1TgSCnhvlCRABHt92oQmWDHDfVyUy%252BLabKS40fLFkOsUK5pTBX30iH3qxPjpy5c700zJ7ovYZ9O3cXEh57PLeAw4vCusAY6sQFvJRLroA9%252Bkm1uDP1HyYx%252FrnZ2I8Gdc4Ew%252Bn%252BIYPNg1MfGY0BvIuGLv%252BQTC3Aezoht5pLeGALjiIxtSlu3kmf2bs8qaQ8VSY6%252B2NiXHiXpNpPhg%252BQ38I6H9wGdSFb4eycVchWna4j44gSTJsmk%252BFI4ylDQiwo2%252FhbeS0M75cE3%252BxpCYohDOLjDGCOm4gKaNBJhsbaQev2sE9UxbVtX4ERqBLAIoOXA8qn%252FMyEr5cE%252B0%252BQ%253D%26X-Amz-Algorithm%3DAWS4-HMAC-SHA256%26X-Amz-Date%3D20240402T085523Z%26X-Amz-SignedHeaders%3Dhost%26X-Amz-Expires%3D300%26X-Amz-Credential%3DASIAQ3PHCVTYWD3YANV7%252F20240402%252Fus-east-1%252Fs3%252Faws4_request%26X-Amz-Signature%3D66b388c73a7d69af8228e98690fd84a85f39ca97d7a17971f8aa744f6aa54059%26hash%3Dbc6d3e603135441cdf1f9d7f0ae9074e5af220eecb7f2470a3e14ba0b0596697%26host%3D68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61%26pii%3DS0952197623005456%26tid%3Dspdf-fa8d856e-3267-4a83-a647-ce18d58a4532%26sid%3D20ee0ed57a6289413b7bb90-eccbb97d3d9egxrqa%26type%3Dclient%26tsoh%3Dd3d3LnNjaWVuY2VkaXJlY3QuY29t%26ua%3D19085d5003045e575c54%26rr%3D86df99843a6c2470%26cc%3Dcn&i=2024-04-02T08%3A55%3A24.253Z&c=pdf_country_code_mismatch&r=86df99887c921fb6&u=https%3A%2F%2Fwww.sciencedirect.com%2F%3Fref%3Dpdf_download%26fr%3DRR-18%26rr%3D86df99887c921fb6&w=interactive&h=eyJrZXkiOiIwNmZzaVZ4MTJjUmExL0JBMGhvTVBnVjEvWStaTUhjZXJza1ZEUFZNWS9qelJJU2kyNzlnQ0ptcjBkNy82WEZVWGRUdnVwZ2V2a2lpdGI2bkowNGl4MjE1bkV0ZUdiUVFNdGtjWDhsZUNWcz0iLCJpdiI6ImU4ZTIwMTdhY2YyMTY3ZjVlNWRkNjhlY2I3YmMxZjk5In0%3D) | Sonain Jamil | Engineering Applications of Artificial Intelligence, 2023 |
| [An Introduction to Neural Data Compression](https://www.nowpublishers.com/article/Download/CGV-107) | Yibo Yang | Foundations and Trends® in Computer Graphics and Vision, 2023 |
| [Learning End-to-End Lossy Image Compression: A Benchmark](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9376651) | Yueyu Hu | TPAMI2022 |
| [Deep architectures for image compression: a critical review](https://pdf.sciencedirectassets.com/271605/1-s2.0-S0165168421X00114/1-s2.0-S0165168421003832/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEBMaCXVzLWVhc3QtMSJHMEUCIQC5GoEqdHliSnucTBBMbDXv%2B5PHcIJVLuMC6MaaZ%2B7gjgIgcNW83SAhurkQmcIPlBl2mt6RblyYCO5iXyxX1GEL8BMqswUIPBAFGgwwNTkwMDM1NDY4NjUiDBiGFlE7X2rwZXp52SqQBS3S7QTeCt02yRDis4PHXcUtzlGWtxBiip8a2UL2Zyz%2BVLQfgfM%2BpJYQ58FxVwieWCXRnWGCPqmGo4jiL9ZMAX1Q9xoS50TpanSo%2Ft8zk7UVLJeKzjh2szeqadbCV1oDo1GTLHK3OjCN%2F15T1%2FqwvbPxXmM75pwqLYaTtv6JC7E4FJNbWByIvTw%2BzC1JpD1COoEaJAmDI3LMMzcAjGHGoebGhL8D2EWC0k33kJhb%2FMBcyxHnuavpQKoZUEOONwKujzqH0nUR%2B6gv4BhgF25xtsMuMLQVKD6Ow5thgxFFxXeYRuHmZ%2FVXKrrQaIK8WIyQvUxMK3ZCzAKkrChnR0wfdE6IDpalslcldWrMDZLVJ1uUrt8tNbSVCmVAEqXnse5QXk6VZLzWhTvsEfdVKSLz6VDf40YmRCLecX%2FhBE9S40V%2BIxV7I7tbkWox46wvB5vuia7x%2Bs5fIQUR3i8BMvI%2B4wfae4XKco8WP5Fjw%2BdsUxpGPcv6Vwr7Ax6oXdx62hXn6fOTYumiB7k5QA%2FVsIsQtboKyAEJfy3r3st8ywM2EcFOGopOcTOOyP2E8d2uh8mJG7ns4vs9lkndxrJSx2gL%2FZb4VWiR5lfT8pUb50x8SVOQHJy68jQdAKSDLJM1a30UzZ1Vsq%2B0Rc1K84s35EyihzVGc8N06Myu%2FL4DOy67AXeLkV3AqL8kubhjN0SvvVvxolWTYskZhBAJvXGbMR5wSBJdN9fI80li%2FzuTne%2FSTHySBjgROs1fU8cXJFcQ9Bq6YnNrosqSyutNPlbPMDwY%2F63QQyH7c4o9wpnwpz2bAqyDTW9OWMQZVmE0xsRMPHPzgn9P8Zz24Ie3hXk9dQy1tQzKfkrF0jbOghFIIoAymL%2FPMP3FqLAGOrEBCUj5qKcNgMvStjY6ud4JdJWPRuESRI8CpGLnOdpGiQOhysC%2FIXFoqUIUMRGifW4gDhT6i68psUdqrov%2FRP7krGNbWYg2Yh9N7M%2BNcI8OK1EZ3lFNf5b%2BU4MmHD893GxtU8F9yruyABT8DFH7Qk2U4n24QzxfY%2BQ3ejGGZbDVVW1PtO%2FRRZCWZiSBesB8fJfzxLqYBxLOQl2uSAMPDvKaz0pAThCO53XLuBXLzbw1UURw&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240401T042211Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYY2KDWSVN%2F20240401%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=dc4d7197bdd66a49e29b7c23d164f9d3090542cf68114ad676a26a0137166cf2&hash=e3a9d9a89a060329beaa3be5baaa68cb6c7d196c18fc4aa5861390e313c898b3&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0165168421003832&tid=spdf-5ccd6e91-7bce-4d5f-9e50-8720de75d2e4&sid=20ee0ed57a6289413b7bb90-eccbb97d3d9egxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=19085d500357040c0105&rr=86d5cbee1ceb8539&cc=cn&kca=eyJrZXkiOiJaVmdGTnFraUUrRTBzVVQwMjZOWDZ3dWU0Z0tUZ1ZXOXY2dXJpRi9uS1F4SEcwSTRxb1VLU3I5SFlZUWlqaXc5U1JKREl6QS9kUS9YZzE4TTIwTzM3eDM1TzV5dmlqL1JmWjZpMlRrd3RYTkpWSDZVNENJTnJLQmI5c2pUaTNFNitOeU1TVUpTWFliL21oQnVvdkljdmNRTVhPOC9INVNBSXlCeUJ5bVRWMVNydy9tb2RRPT0iLCJpdiI6ImQ0YWY0ZTk5OTBiZmI4ODkyYjA4ZTAxNDZhYTE1MzBkIn0=_1711945335528) | Dipti Mishra | Signal Processing, 2022 |
| [Image and Video Compression With Neural Networks: A Review](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8693636) | Siwei Ma | TCSVT2019 |
| [A comprehensive survey on image encryption: Taxonomy, challenges, and future directions](https://www.sciencedirect.com/science/article/pii/S0960077923012638?via%3Dihub) | Morteza SaberiKamarposhti | Chaos, Solitons and Fractals, 2024 |

## Lossless Image Compression
|Models| Paper | First Author | Venue | Project |
| :--: | :---: | :--: | :--:| :--: |
|LC-FDNet| [LC-FDNet: Learned Lossless Image Compression With Frequency Decomposition Network](https://openaccess.thecvf.com/content/CVPR2022/papers/Rhee_LC-FDNet_Learned_Lossless_Image_Compression_With_Frequency_Decomposition_Network_CVPR_2022_paper.pdf) | Hochang Rhee | CVPR2022 | [![Stars](https://img.shields.io/github/stars/myideaisgood/LC-FDNet.svg?style=social&label=Star)](https://github.com/myideaisgood/LC-FDNet) |
|PILC| [PILC: Practical Image Lossless Compression With an End-to-End GPU Oriented Neural Framework](https://openaccess.thecvf.com/content/CVPR2022/papers/Kang_PILC_Practical_Image_Lossless_Compression_With_an_End-to-End_GPU_Oriented_CVPR_2022_paper.pdf) | Ning Kang, Shanzhao Qiu | CVPR2022 |  |
|IDF++| [IDF++: Analyzing and Improving Integer Discrete Flows for Lossless Compression](https://openreview.net/forum?id=MBOyiNnYthd) | Rianne van den Berg | ICLR2021 |  |
|iFlow| [iFlow: Numerically Invertible Flows for Efficient Lossless Compression via a Uniform Coder](https://arxiv.org/abs/2111.00965) | Shifeng Zhang | NeurIPS2021 |  |
|OSOA| [OSOA: One-Shot Online Adaptation of Deep Generative Models for Lossless Compression](https://arxiv.org/abs/2111.01662) | Chen Zhang | NeurIPS2021 |  |
| -- | [Improving Lossless Compression Rates via Monte Carlo Bits-Back Coding](https://arxiv.org/abs/2102.11086) | Yangjun Ruan, Karen Ullrich | ICML2021 | [![Stars](https://img.shields.io/github/stars/ryoungj/mcbits.svg?style=social&label=Star)](https://github.com/ryoungj/mcbits) |
|iVPF| [iVPF: Numerical Invertible Volume Preserving Flow for Efficient Lossless Compression](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_iVPF_Numerical_Invertible_Volume_Preserving_Flow_for_Efficient_Lossless_Compression_CVPR_2021_paper.pdf) | Shifeng Zhang | CVPR2021 |  |
| -- | [Learning Scalable l∞-constrained Near-lossless Image Compression via Joint Lossy Image and Residual Compression](https://openaccess.thecvf.com/content/CVPR2021/papers/Bai_Learning_Scalable_lY-Constrained_Near-Lossless_Image_Compression_via_Joint_Lossy_Image_CVPR_2021_paper.pdf) | Yuanchao Bai | CVPR2021 |  [![Stars](https://img.shields.io/github/stars/BYchao100/Scalable-Near-lossless-Image-Compression.svg?style=social&label=Star)](https://github.com/BYchao100/Scalable-Near-lossless-Image-Compression) |
|L3C| [Practical full resolution learned lossless image compression](https://openaccess.thecvf.com/content_CVPR_2019/papers/Mentzer_Practical_Full_Resolution_Learned_Lossless_Image_Compression_CVPR_2019_paper.pdf) | Fabian Mentzer | CVPR2019 | [![Stars](https://img.shields.io/github/stars/fab-jul/L3C-PyTorch.svg?style=social&label=Star)](https://github.com/fab-jul/L3C-PyTorch) |


## Near-Lossless Image Compression
|Models| Paper | First Author | Architecture | Venue | Project |
| :--: | :---: | :--: | :--: | :--: | :--: |
| -- | [Ultra High Fidelity Deep Image Decompression With l∞-Constrained Compression](https://ieeexplore.ieee.org/document/9277919) | Xi Zhang | CNN | TIP2020 | |
| -- | [Learning Scalable l∞-constrained Near-lossless Image Compression via Joint Lossy Image and Residual Compression](https://openaccess.thecvf.com/content/CVPR2021/papers/Bai_Learning_Scalable_lY-Constrained_Near-Lossless_Image_Compression_via_Joint_Lossy_Image_CVPR_2021_paper.pdf) | Yuanchao Bai | VAE | CVPR2021 |  [![Stars](https://img.shields.io/github/stars/BYchao100/Scalable-Near-lossless-Image-Compression.svg?style=social&label=Star)](https://github.com/BYchao100/Scalable-Near-lossless-Image-Compression) |
| DLPR | [Deep Lossy Plus Residual Coding for Lossless and Near-lossless Image Compression](https://ieeexplore.ieee.org/document/10378746) | Yuanchao Bai | VAE | TPAMI2023 |  [![Stars](https://img.shields.io/github/stars/BYchao100/Deep-Lossy-Plus-Residual-Coding.svg?style=social&label=Star)](https://github.com/BYchao100/Deep-Lossy-Plus-Residual-Coding) |





## Lossy Image Compression
### Nonlinear Transform Coding
|Models| Paper | First Author | Architecture | Venue | Project |
| :--: | :---: | :--: | :--:| :--: | :--: |
| -- | [Learned Image Compression with Mixed Transformer-CNN Architectures](https://openaccess.thecvf.com/content/CVPR2023/papers/Liu_Learned_Image_Compression_With_Mixed_Transformer-CNN_Architectures_CVPR_2023_paper.pdf) | Jinming Liu | AE | CVPR2023 | [![Stars](https://img.shields.io/github/stars/jmliu206/LIC_TCM.svg?style=social&label=Star)](https://github.com/jmliu206/LIC_TCM) |
| NVTC | [NVTC: Nonlinear Vector Transform Coding](https://openaccess.thecvf.com/content/CVPR2023/papers/Feng_NVTC_Nonlinear_Vector_Transform_Coding_CVPR_2023_paper.pdf) | Runsen Feng |  | CVPR2023 | [![Stars](https://img.shields.io/github/stars/USTC-IMCL/NVTC.svg?style=social&label=Star)](https://github.com/USTC-IMCL/NVTC) |
| ELIC | [ELIC: Efficient Learned Image Compression with Unevenly Grouped Space-Channel Contextual Adaptive Coding](https://arxiv.org/abs/2203.10886) | Dailan He |  | CVPR2022 | |
| SHVQ | [Soft-to-Hard Vector Quantization for End-to-End Learning Compressible Representations](https://proceedings.neurips.cc/paper_files/paper/2017/file/86b122d4358357d834a87ce618a55de0-Paper.pdf) | Eirikur Agustsson | AE | NIPS2017 |  |
| -- | [Lossy Image Compression with Compressive Autoencoders](https://openreview.net/pdf?id=rJiNwv9gg) | Lucas Theis | AE | ICLR2017 |  |
| -- | [End-to-end Optimized Image Compression](https://arxiv.org/pdf/1611.01704.pdf) | Johannes Ballé | AE | ICLR2017 | [![Stars](https://img.shields.io/github/stars/tensorflow/compression.svg?style=social&label=Star)](https://github.com/tensorflow/compression) |
| -- | [Few-Shot Domain Adaptation for Learned Image Compression](https://arxiv.org/pdf/2409.11111) | Tianyu Zhang | AE | Arxiv2024 |  |

### Generative Image compression
<!-- TODO: Ruixin -->
|Models| Paper | First Author | Architecture | Venue | Project |
| :--: | :---: | :--: | :--: | :--: | :--: |
| CDC | [Lossy Image Compression with Conditional Diffusion Models](https://proceedings.neurips.cc/paper_files/paper/2023/file/ccf6d8b4a1fe9d9c8192f00c713872ea-Paper-Conference.pdf) | Ruihan Yang | Diffusion Model | NeurIPS2023 | [![Stars](https://img.shields.io/github/stars/buggyyang/CDC_compression.svg?style=social&label=Star)](https://github.com/buggyyang/CDC_compression) |
| HiFiC | [High-Fidelity Generative Image Compression](https://proceedings.neurips.cc/paper_files/paper/2020/file/8a50bae297807da9e97722a0b3fd8f27-Paper.pdf) | Fabian Mentzer | GAN | NeurIPS2020 | [![Stars](https://img.shields.io/github/stars/tensorflow/compression.svg?style=social&label=Star)](https://github.com/tensorflow/compression/tree/master/models/hific) |
| -- | [Rethinking Lossy Compression: The Rate-Distortion-Perception Tradeoff](https://proceedings.mlr.press/v97/blau19a/blau19a.pdf) | Yochai Blau | -- | ICML2019 |  |

## Other tasks
### Encryption
| Methods | Paper | First Author | Venue |
| :--: | :---: | :--: | :--: |
| Visual Cryptography | [Dynamic feedback bit‑level image privacy protection based on chaos and information hiding](https://www.nature.com/articles/s41598-024-53325-4) | Jinlong Zhang | scientific Reports, 2024 |
| CS | [A multi-level privacy-preserving scheme for extracting traffic images](https://www.sciencedirect.com/science/article/pii/S0165168424000641) | Xiaofei He | Signal Processing, 2024 |
| DNA | [A novel image compression and encryption scheme based on conservative chaotic system and DNA method](https://www.sciencedirect.com/science/article/pii/S0960077923003934?via%3Dihub) | Xin Wu | Chaos, Solitons and Fractals, 2023 |

## Uncategorized Papers
| Models | Paper | First Author | Venue | Project |
| :--: | :---: | :--: | :--: | :--: |
|  | [Approximately Invertible Neural Network for Learned Image Compression](https://arxiv.org/pdf/2408.17073) | Yanbo Gao | arXiv 2024.08 |  |
|  | [A Unified Image Compression Method for Human Perception and Multiple Vision Tasks](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/09009.pdf) | Sha Guo* , Lin Sui* | ECCV 2024 |  |
|  | [BaSIC: BayesNet Structure Learning for Computational Scalable Neural Image Compression](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/03640.pdf) | Yufeng Zhang | ECCV 2024 | [![GitHub Repo stars](https://img.shields.io/github/stars/worldlife123/cbench_BaSIC)](https://github.com/worldlife123/cbench_BaSIC) |
|  | [Few-Shot Domain Adaptation for Learned Image Compression](https://arxiv.org/pdf/2409.11111) | Tianyu Zhang | arXiv 2024.09 |  |
|  | [Window-based Channel Attention for Wavelet-enhanced Learned Image Compression](https://arxiv.org/pdf/2409.14090) | Heng Xu | arXiv 2024.09 |  |
|  | [Diffusion-based Extreme Image Compression with Compressed Feature Initialization](https://arxiv.org/pdf/2410.02640) | Zhiyuan Li | arXiv 2024.10 |  |
|  | [Causal Context Adjustment Loss for Learned Image Compression](https://arxiv.org/pdf/2410.04847) | Minghao Han | NeurIPS 2024 |  |
|  | [Fast Feedforward 3D Gaussian Splatting Compression](https://arxiv.org/pdf/2410.08017) | Yihang Chen | arXiv 2024.10 |  |
|  | [DeepHQ: Learned Hierarchical Quantizer for Progressive Deep Image Coding](https://arxiv.org/pdf/2408.12150) | Jooyoung Lee | arXiv 2024.08 |  |
|  | [Tell Codec What Worth Compressing: Semantically Disentangled Image Coding for Machine with LMMs](https://arxiv.org/pdf/2408.08575) | Jinming Liu | arXiv 2024.08 |  |
|  | [Bi-Level Spatial and Channel-aware Transformer for Learned Image Compression](https://arxiv.org/pdf/2408.03842) | Hamidreza Soltani | 2024.08 |  |
|  | [Bidirectional Stereo Image Compression with Cross-Dimensional Entropy Model](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/01341.pdf) | Zhening Liu | ECCV 2024 |  |
|  | [Rate-Distortion-Cognition Controllable Versatile Neural Image Compression](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/07338.pdf) | Jinming Liu | ECCV 2024 |  |
|  | [Image Compression for Machine and Human Vision With Spatial-Frequency Adaptation](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06823.pdf) | Han Li | ECCV 2024 |  |
|  | [Rethinking Learned Image Compression: Context is All You Need](https://arxiv.org/pdf/2407.11590) | Jixiang Luo | arXiv 2024.07 |  |
|  | [High Frequency Matters: Uncertainty Guided Image Compression with Wavelet Diffusion](https://arxiv.org/pdf/2407.12538) | Juan Song | arXiv 2024.07 |  |
|  | [High Efficiency Image Compression for Large Visual-Language Models](https://arxiv.org/pdf/2407.17060) | Binzhe Li | arXiv 2024.07 |  |
|  | [WeConvene: Learned Image Compression with Wavelet-Domain Convolution and Entropy Model](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06635.pdf) | Haisheng Fu | ECCV 2024 |  |
|  | [Learned HDR Image Compression for Perceptually Optimal Storage and Display](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06526.pdf) | Peibei Cao | ECCV 2024 |  |
|  | [ComNeck: Bridging Compressed Image Latents and Multimodal LLMs via Universal Transform-Neck](https://arxiv.org/pdf/2407.19651) | Chia-Hao Kao | arXiv 2024.07 |  |
|  | [3DGS.zip: A survey on 3D Gaussian Splatting Compression Methods](https://arxiv.org/pdf/2407.09510) | Milena T. Bagdasarian | arXiv 2024.07 |  |
|  | [WHICH TASKS SHOULD BE COMPRESSED TOGETHER? A CAUSAL DISCOVERY APPROACH FOR EFFICIENT MULTI-TASK REPRESENTATION COMPRESSION](https://openreview.net/forum?id=x33vSZUg0A)) |  | ICLR 2025 Conference Submission |  |
|  | [Large Language Model for Lossless Image Compression with Visual Prompts](https://openreview.net/forum?id=dcG17rjJF9) |  | ICLR 2025 Conference Submission |  |
|  | [TEST-TIME ADAPTATION FOR IMAGE COMPRESSION WITH DISTRIBUTION REGULARIZATION](https://openreview.net/forum?id=bsnRUkVn63) |  | ICLR 2025 Conference Submission |  |
