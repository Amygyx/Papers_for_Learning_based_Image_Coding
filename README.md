# Papers for Neural Image Compression
**Purpose:** We aim to provide a summary of neural image compression. More papers will be summarized. 

University of Science and Technology of China (USTC), [Intelligent Media Computing Lab](https://faculty.ustc.edu.cn/chenzhibo).

**📌 About new works.** If you want to incorporate your studies (e.g., the link of paper or project) on neural image compression in this repository. Welcome to raise an issue or email us. We will incorporate it into this repository and our survey report as soon as possible.

## Table of contents
- [Survey](#Survey)
- [Lossless Image Compression](#lossless-image-compression)
- [Near-Lossless Image Compression](#near-lossless-image-compressio)
- [Lossy Image Compression](#lossy-image-compression)
  - [Nonlinear Transform Coding](#nonlinear-transform-coding)
    - [2015](#2015)
  - [Generative Image compression](#generative-image-compression)
- [Other tasks](#other-tasks)
<!-- variable rate, adjustable complexity, scalable coding, light field, stereo image and so on  -->
<!--   - [RNN-style](#RNN-style)
  - [VAE-style](#VAE-style)
  - [INR-style](#INR-style)
  - [Invertible transform style](#Invertible-transform-style) -->

## Survey
<!-- TODO: Ruixin  -->
| Paper | First Author | Venue | 
| :---: | :--: | :--:|
| [Deep architectures for image compression: a critical review](https://pdf.sciencedirectassets.com/271605/1-s2.0-S0165168421X00114/1-s2.0-S0165168421003832/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEBMaCXVzLWVhc3QtMSJHMEUCIQC5GoEqdHliSnucTBBMbDXv%2B5PHcIJVLuMC6MaaZ%2B7gjgIgcNW83SAhurkQmcIPlBl2mt6RblyYCO5iXyxX1GEL8BMqswUIPBAFGgwwNTkwMDM1NDY4NjUiDBiGFlE7X2rwZXp52SqQBS3S7QTeCt02yRDis4PHXcUtzlGWtxBiip8a2UL2Zyz%2BVLQfgfM%2BpJYQ58FxVwieWCXRnWGCPqmGo4jiL9ZMAX1Q9xoS50TpanSo%2Ft8zk7UVLJeKzjh2szeqadbCV1oDo1GTLHK3OjCN%2F15T1%2FqwvbPxXmM75pwqLYaTtv6JC7E4FJNbWByIvTw%2BzC1JpD1COoEaJAmDI3LMMzcAjGHGoebGhL8D2EWC0k33kJhb%2FMBcyxHnuavpQKoZUEOONwKujzqH0nUR%2B6gv4BhgF25xtsMuMLQVKD6Ow5thgxFFxXeYRuHmZ%2FVXKrrQaIK8WIyQvUxMK3ZCzAKkrChnR0wfdE6IDpalslcldWrMDZLVJ1uUrt8tNbSVCmVAEqXnse5QXk6VZLzWhTvsEfdVKSLz6VDf40YmRCLecX%2FhBE9S40V%2BIxV7I7tbkWox46wvB5vuia7x%2Bs5fIQUR3i8BMvI%2B4wfae4XKco8WP5Fjw%2BdsUxpGPcv6Vwr7Ax6oXdx62hXn6fOTYumiB7k5QA%2FVsIsQtboKyAEJfy3r3st8ywM2EcFOGopOcTOOyP2E8d2uh8mJG7ns4vs9lkndxrJSx2gL%2FZb4VWiR5lfT8pUb50x8SVOQHJy68jQdAKSDLJM1a30UzZ1Vsq%2B0Rc1K84s35EyihzVGc8N06Myu%2FL4DOy67AXeLkV3AqL8kubhjN0SvvVvxolWTYskZhBAJvXGbMR5wSBJdN9fI80li%2FzuTne%2FSTHySBjgROs1fU8cXJFcQ9Bq6YnNrosqSyutNPlbPMDwY%2F63QQyH7c4o9wpnwpz2bAqyDTW9OWMQZVmE0xsRMPHPzgn9P8Zz24Ie3hXk9dQy1tQzKfkrF0jbOghFIIoAymL%2FPMP3FqLAGOrEBCUj5qKcNgMvStjY6ud4JdJWPRuESRI8CpGLnOdpGiQOhysC%2FIXFoqUIUMRGifW4gDhT6i68psUdqrov%2FRP7krGNbWYg2Yh9N7M%2BNcI8OK1EZ3lFNf5b%2BU4MmHD893GxtU8F9yruyABT8DFH7Qk2U4n24QzxfY%2BQ3ejGGZbDVVW1PtO%2FRRZCWZiSBesB8fJfzxLqYBxLOQl2uSAMPDvKaz0pAThCO53XLuBXLzbw1UURw&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20240401T042211Z&X-Amz-SignedHeaders=host&X-Amz-Expires=300&X-Amz-Credential=ASIAQ3PHCVTYY2KDWSVN%2F20240401%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=dc4d7197bdd66a49e29b7c23d164f9d3090542cf68114ad676a26a0137166cf2&hash=e3a9d9a89a060329beaa3be5baaa68cb6c7d196c18fc4aa5861390e313c898b3&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0165168421003832&tid=spdf-5ccd6e91-7bce-4d5f-9e50-8720de75d2e4&sid=20ee0ed57a6289413b7bb90-eccbb97d3d9egxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=19085d500357040c0105&rr=86d5cbee1ceb8539&cc=cn&kca=eyJrZXkiOiJaVmdGTnFraUUrRTBzVVQwMjZOWDZ3dWU0Z0tUZ1ZXOXY2dXJpRi9uS1F4SEcwSTRxb1VLU3I5SFlZUWlqaXc5U1JKREl6QS9kUS9YZzE4TTIwTzM3eDM1TzV5dmlqL1JmWjZpMlRrd3RYTkpWSDZVNENJTnJLQmI5c2pUaTNFNitOeU1TVUpTWFliL21oQnVvdkljdmNRTVhPOC9INVNBSXlCeUJ5bVRWMVNydy9tb2RRPT0iLCJpdiI6ImQ0YWY0ZTk5OTBiZmI4ODkyYjA4ZTAxNDZhYTE1MzBkIn0=_1711945335528) | Dipti Mishra | Signal Processing, 2022 |

## Lossless Image Compression
|Models| Paper | First Author | Venue | Project |
| :--: | :---: | :--: | :--:| :--: |
|L3C| [Practical full resolution learned lossless image compression](https://openaccess.thecvf.com/content_CVPR_2019/papers/Mentzer_Practical_Full_Resolution_Learned_Lossless_Image_Compression_CVPR_2019_paper.pdf) | Fabian Mentzer | CVPR2019 | [![Stars](https://img.shields.io/github/stars/fab-jul/L3C-PyTorch.svg?style=social&label=Star)](https://github.com/fab-jul/L3C-PyTorch) |


## Near-Lossless Image Compression
<!-- TODO: xiaoshuai  -->
|Models| Paper | First Author | Architecture | Venue | Project |
| :--: | :---: | :--: | :--: | :--: | :--: |
| -- | [Learning Scalable `∞-constrained Near-lossless Image Compression via Joint Lossy Image and Residual Compression](https://openaccess.thecvf.com/content/CVPR2021/papers/Bai_Learning_Scalable_lY-Constrained_Near-Lossless_Image_Compression_via_Joint_Lossy_Image_CVPR_2021_paper.pdf) | Yuanchao Bai | VAE | CVPR2021 |  [![Stars]([https://img.shields.io/github/stars/tensorflow/compression.svg?style=social&label=Star)](https://github.com/tensorflow/compression/tree/master/models/hific](https://github.com/BYchao100/Scalable-Near-lossless-Image-Compression)) |




## Lossy Image Compression
### Nonlinear Transform Coding
#### 2015
|Models| Paper | First Author | Venue | Project |
| :--: | :---: | :--: | :--:| :--: |
| -- | [Variable Rate Image Compression with Recurrent Neural Networks](https://openaccess.thecvf.com/content_CVPR_2019/papers/Mentzer_Practical_Full_Resolution_Learned_Lossless_Image_Compression_CVPR_2019_paper.pdf) | Fabian Mentzer | CVPR2019 |  |

### Generative Image compression
|Models| Paper | First Author | Architecture | Venue | Project |
| :--: | :---: | :--: | :--: | :--: | :--: |
| HiFiC | [High-Fidelity Generative Image Compression](https://proceedings.neurips.cc/paper_files/paper/2020/file/8a50bae297807da9e97722a0b3fd8f27-Paper.pdf) | Fabian Mentzer | GAN | NeurIPS2020 | [![Stars](https://img.shields.io/github/stars/tensorflow/compression.svg?style=social&label=Star)](https://github.com/tensorflow/compression/tree/master/models/hific) |
| -- | [Rethinking Lossy Compression: The Rate-Distortion-Perception Tradeoff](https://proceedings.mlr.press/v97/blau19a/blau19a.pdf) | Yochai Blau | -- | ICML2019 |  |

## Other tasks
