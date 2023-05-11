共測試三台設備 安裝並跑過這些專案

全部環境已 miniconda3 來做跨平台轉移

1.MSI PS63 NB / Windows 10 22H2
  GPU:Nvidia GTX-1050<cr>
  CUDA:11.5<cr>
  cudNN:8.3<cr>
  Tensorflow-gpu=2.1.0<cr>
  Pytorch:1.4<cr>
  conda create --name p01 python=3.7.12<cr>
  pip install -r p01.env<cr>

2.PC AMD / Windows 10<cr>
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
 
