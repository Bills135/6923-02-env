共測試三台設備 安裝並跑過這些專案

全部環境已 miniconda3 來做跨平台轉移

1.MSI PS63 NB / Windows 10 22H2  
  GPU:Nvidia GTX-1050  
  CUDA:11.5  
  cudNN:8.3  
  Tensorflow-gpu=2.1.0  
  Pytorch:1.4  
  conda create --name p01 python=3.7.12  
  pip install -r p01.env  

2.PC AMD / Windows 10  
   GPU:Nvidia GTX-1660S  
  CUDA:11.5  
  cudNN:8.3  
  Tensorflow-gpu=2.1.0  
  Pytorch:1.4  
  conda create --name p01 python=3.7.12  
  pip install -r p01.env  
 
3.Linux Server / Ubuntu Server 2023.04  
  GPU:RTX-3060-12GB  
  CUDA:12.1  
  cudNN  
 Tensorflow-gpu=2.1.0  
  Pytorch:1.4  
  conda create --name p01 python=3.7.6  
  pip install -r p01.env  
 
============================================   

由於學生朝向醫療方向在學習 ，因此擬定三篇論文做測試  
1.  
JCS: An Explainable COVID-19 Diagnosis System by Joint Classification and Segmentation(2020)  
https://ieeexplore.ieee.org/document/9357961  
Code : https://github.com/yuhuan-wu/JCS  

2.  
Inf-Net: Automatic COVID-19 Lung Infection Segmentation from CT Images (2020)  
https://arxiv.org/abs/2004.14133  
Code : https://github.com/DengPingFan/Inf-Net/pulls  

3.  
ECG Heartbeat Classification: A Deep Transferable Representation (2018)  
https://ieeexplore.ieee.org/document/8419425  
2018 IEEE International Conference on Healthcare Informatics (ICHI)  
Code : https://paperswithcode.com/paper/ecg-heartbeat-classification-a-deep  