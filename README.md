# DITNet
Refined Feature Alignment and Dynamic Interaction Transformer for Multispectral Pedestrian Detection

## **Overview**
<p align="center">
  <img src="README.assets\image-20240312011746031.png" alt="overview" width="90%">
</p>


## **Getting Started**
### Step 1: Clone the DITNet repository:

***To get started, first clone the DITNet repository and navigate to the project directory:***

```bash
git clone https://github.com/12lele/DITNet.git
cd DITNet
```
### Step 2: Environment Setup:

***Create a virtual environment using conda*** 

```bash
conda create -n DITNet python=3.8 -y
conda activate DITNet
```

***Install dependencies.Pay attention to whether your CUDA and TORCH match*** 

```bash
pip install torch==1.13.0+cu117 torchvision==0.14.0+cu117 torchaudio==0.13.0 --extra-index-url https://download.pytorch.org/whl/cu117
pip install -r requirements.txt
```

### Step 3: Download dataset:
Please note that the corresponding path needs to be modified in the file under data/multispectral

***Kaist Dataset:***

 ```bash
Link：https://pan.baidu.com/s/1bECsaWaeWd_4DJIhO8S2Og?pwd=5lz0 code：5lz0
```

***FLIR Dataset:***

 ```bash
Link:https://pan.baidu.com/s/14BKgDguo5Z9UGBzPT9P73w?pwd=aipo code：aipo
```

### Step 4: Download weight:

***Kaist Weight:***
 ```bash
Link: https://pan.baidu.com/s/1SzHaj8Xg-LRyciRJsnrUHQ?pwd=rvwq code: rvwq
```
***FLIR Weight:***
 ```bash
Link：https://pan.baidu.com/s/1Hnl6aYkoVnOsLCLEUBewew?pwd=l442 code：l442
```


### Step 5: Run the test file:
***Kaist:***
 ```bash
python test_kaist.py
 ```
***FLIR:***
 ```bash
python test_FLIR.py
 ```
### If you want to train your own network to obtain your own weights, you can use the following command


 ```bash
CUDA_VISIBLE_DEVICES=0 python train_kaist.py 
```
