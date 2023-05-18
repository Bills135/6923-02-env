共測試三台設備 安裝並跑過這些專案

全部環境已 miniconda3 來做跨平台轉移
|		|pc				|nb				|LinuxServer|
|---------------|:-----------------------------:|:-----------------------------:|:---------------------------:|
|6923-03-JCS	|torch 1.13/0.13.1/0.14.1	|torch 1.13/0.13.1/0.14.1	|torch 1.13/0.13.1/0.14.1|
|6923-04-Inf-net	|torch 1.13/0.13.1/0.14.1	|torch 1.13/0.13.1/0.14.1	|torch 1.13/0.13.1/0.14.1|
|6923-05-ECG	|tensorflow-gpu=2.11.0		|tensorflow-gpu=2.6.0		|tensorflow-gpu=2.6.0|

|pytorch		|Version|
|-----------------------|--------|
|torch              	|1.13.1|
|torchaudio         	|0.13.1|
|torchvision        	|0.14.1|

|1.MSI PS63 NB / Windows 10 22H2|		|			|		|
|-------------------------------|---------------|-----------------------|---------------|
|python                    	|3.7.12         |h900ac77_100_cpython   |conda-forge	|
|pytorch                   	|1.13.1         |py3.7_cpu_0    	|pytorch	|
|pytorch-mutex             	|1.0            |cpu    		|pytorch	|
|torchvision               	|0.13.1		|			|		|

pip install torch==1.13.0 torchvision -f https://download.pytorch.org/whl/torch_stable.html			

|tensorflow                	|2.11.0     |
|-------------------------------|-----------|
|tensorflow-estimator      	|2.0.1      |
|tensorflow-gpu            	|2.0.0      |
|tensorflow-intel          	|2.11.0     |
|tensorflow-io-gcs-filesystem 	|0.31.0     |

conda create --name gpu tensorflow-gpu=2.0.0 python=3.7.12  
##
nvcc: NVIDIA (R) Cuda compiler driver  
Copyright (c) 2005-2018 NVIDIA Corporation  
Built on Sat_Aug_25_21:08:04_Central_Daylight_Time_2018  
Cuda compilation tools, release 10.0, V10.0.130  
  
2.PC AMD / Windows 10  
   GPU:Nvidia GTX-1660S  
   CUDA:11.5  
   cudNN:8.3  

|tensorflow               |2.1.0|
|-------------------------|-----|
|tensorflow-estimator     |2.5.0|
|tensorflow-gpu           |2.5.0|
|tensorflow-gpu-estimator |2.3.0|

nvcc: NVIDIA (R) Cuda compiler driver  
Copyright (c) 2005-2021 NVIDIA Corporation  
Built on Thu_Nov_18_09:52:33_Pacific_Standard_Time_2021  
Cuda compilation tools, release 11.5, V11.5.119  
Build cuda_11.5.r11.5/compiler.30672275_0  

3.Linux Server / Ubuntu Server 2023.04  
tensorflow = 2.6.0  
python=3.7.16  

  |- pytorch=1.13.1=py3.7_cuda11.7_cudnn8.5.0_0   	|
  |-----------------------------------------------------|
  |- pytorch-cuda=11.7=h778d358_3   			|
  |- torchaudio=0.13.1=py37_cu117   			|
  |- torchvision=0.14.1=py37_cu117   			|

|torch              	|1.13.1|
|-----------------------|------|
|torchaudio         	|0.13.1|
|torchvision        	|0.14.1|

nvcc: NVIDIA (R) Cuda compiler driver   
Copyright (c) 2005-2022 NVIDIA Corporation   
Built on Wed_Sep_21_10:33:58_PDT_2022   
Cuda compilation tools, release 11.8, V11.8.89   
Build cuda_11.8.r11.8/compiler.31833905_0   
  
***  

由於學生朝向醫療方向在學習 ，因此擬定三篇論文做測試   
##1.  
JCS: An Explainable COVID-19 Diagnosis System by Joint Classification and Segmentation(2020)  
https://ieeexplore.ieee.org/document/9357961  
Code : https://github.com/yuhuan-wu/JCS  

##2.  
Inf-Net: Automatic COVID-19 Lung Infection Segmentation from CT Images (2020)  
https://arxiv.org/abs/2004.14133  
Code : https://github.com/DengPingFan/Inf-Net/pulls  

##3.  
ECG Heartbeat Classification: A Deep Transferable Representation (2018)  
https://ieeexplore.ieee.org/document/8419425  
2018 IEEE International Conference on Healthcare Informatics (ICHI)  
Code : https://paperswithcode.com/paper/ecg-heartbeat-classification-a-deep  