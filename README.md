# Pytorch-on-jetson-nano
## How to install Pytorch on Nividia Jetson Nano
  install the dependencies (if not already onboard)    
> ``` $ sudo apt-get install python3-pip libjpeg-dev libopenblas-dev libopenmpi-dev libomp-dev ```  
> ``` $ sudo -H pip3 install future ```  
> ``` $ sudo pip3 install -U --user wheel mock pillow ```  
> ``` $ sudo -H pip3 install testresources ```
## Upgrade setuptools 47.1.1 -> 57.4.0'  
> ``` $ sudo -H pip3 install --upgrade setuptools ```  
> ``` $ sudo -H pip3 install Cython ```  
## Install gdown to download from Google drive    
> ``` $ sudo -H pip3 install gdown ```   
## Download the wheel  
> ``` $ gdown https://drive.google.com/uc?id=12UiREE6-o3BthhpjQxCKLtRg3u4ssPqb ```  
## Install PyTorch 1.9.0  
> ```$ sudo -H pip3 install torch-1.9.0a0+gitd69c22d-cp36-cp36m-linux_aarch64.whl ```  
## Error     
 import torch as tr  
Illegal instruction (core dumped)  
 Solution [https://forums.developer.nvidia.com/t/illegal-instruction-core-dumped/165488]

## Clean up  
> ```$ rm torch-1.9.0a0+gitd69c22d-cp36-cp36m-linux_aarch64.whl ```
