# PRISM: Motion Deblurring with RGB and Event Cameras

This repository contains the official implementation of our work on motion deblurring using RGB and event cameras.  
Training scripts and pretrained weights will be released after the paper is accepted.  

---

## Installation  

This project is built on [BasicSR](https://github.com/xinntao/BasicSR).  

**Requirements:**  
- Python >= 3.8  
- PyTorch >= 1.7.1  
- CUDA >= 11.0  

```bash
git clone https://github.com/yourusername/PRISM
cd PRISM
pip install -r requirements.txt
python setup.py develop --no_cuda_ext
```

---

## Dataset  

We evaluate our method on the following datasets:  
- **GoPro** (synthetic motion blur)  
- **REBlur** (real event-based blur)  
- **HighREV** (real-world challenging scenarios)  


Place the datasets under:  

```
./datasets/DATASET_NAME/train/
./datasets/DATASET_NAME/test/
```

---

## Quick Start  

Example command to launch training (dataset and config file required):  

```bash
python basicsr/train.py -opt options/train/GoPro/PRISM.yml
```

---

More training scripts and pretrained models will be released after the paper is accepted.  
