# HDR-CNF: Single-Image High Dynamic Range Imaging based on Conditional Normalizing Flows

By Kai-Wei Peng, Jui-Chiu Chiang<sup>*</sup>, Sau-Gee Chen and Yu-Shan Lin

## Abstract 
We present HDR-CNF, a novel method for reconstructing high dynamic range (HDR) images from single low dynamic range (LDR) images using conditional normalizing flows. Our approach takes advantage of the invertibility provided by normalizing flows and leverages the stability of negative log-likelihood loss to efficiently transform the conditional distribution of HDR images given LDR images into a Gaussian distribution. During inference, we successfully generate an HDR image by sampling from the Gaussian distribution along with the corresponding LDR image. To conditionally input the LDR image, we employ a feature extraction network to extract rich features, enhancing the network's ability to generate high-quality HDR images. Furthermore, we introduce a cycle consistency loss to ensure that the generated HDR images closely resemble the authentic HDR images. Comparative evaluations demonstrate the superiority of our method over existing HDR imaging techniques. Our approach excels in reconstructing well-exposed LDR images into satisfactory HDR images and enhances slightly under-exposed or over-exposed LDR images, outperforming other methods in terms of image quality. In addition to performance evaluations, we conduct a comprehensive analysis of the complexity of our network architecture. Our results showcase impressive performance across various evaluation metrics, providing compelling evidence of the effectiveness of HDR-CNF in HDR image reconstruction.
![Network](https://github.com/shan496/HDR-CNF/blob/main/image/Figure.1.jpg)


## Environments

* CUDA 11.2 on Ubuntu 20.04
* Python 3.7.11
* PyTorch 1.7.0+cu110
* Torchvision 0.8.1+cu110

## Dataset
*  You can download the dataset from [SingleHDR](https://alex04072000.github.io/SingleHDR/) for training and testing.


## Results
![results](https://github.com/shan496/HDR-CNF/blob/main/image/result_2.jpg)


## Acknowledgement
Our work is inspired the following works and uses parts of their official implementations:

* [SRFlow](https://github.com/andreas128/SRFlow)
* [SingleHDR](https://alex04072000.github.io/SingleHDR/)

We thank the respective authors for open sourcing their methods.

