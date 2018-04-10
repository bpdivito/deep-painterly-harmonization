# deep-painterly-harmonization
Code and data for paper "Deep Photo Harmonization". (Arxiv link: coming soon) 

## Disclaimer 
**This software is published for academic and non-commercial use only.**

## Setup
This code is based on torch. It has been tested on Ubuntu 16.04 LTS.

Dependencies:
* [Torch](https://github.com/torch/torch7) (with [loadcaffe](https://github.com/szagoruyko/loadcaffe))
* [Matlab](https://www.mathworks.com/) or [Octave](https://www.gnu.org/software/octave/)

CUDA backend:
* [CUDA](https://developer.nvidia.com/cuda-downloads)
* [cudnn](https://developer.nvidia.com/cudnn)

Download VGG-19:
```
sh models/download_models.sh
```

Compile ``cuda_utils.cu`` (Adjust ``PREFIX`` and ``NVCC_PREFIX`` in ``makefile`` for your machine):
```
make clean && make
```

## Usage
### Quick start
To generate all results (in  ``data/``) using the provided scripts, simply run
```
python gen_all.py
```
in Python and then 
```
run('filt_cnn_artifact.m')
```
in Matlab or Octave. The final output will be in ``results/``.

## Examples
Here are some results from our algorithm (from left to right are original painting, naive composite and our output):
<p align='center'>
  <img src='data/0_naive.jpg' width='435'/>
  <img src='results/0_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/1_naive.jpg' width='435'/>
  <img src='results/1_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/2_naive.jpg' width='435'/>
  <img src='results/2_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/3_naive.jpg' width='435'/>
  <img src='results/3_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/4_naive.jpg' width='435'/>
  <img src='results/4_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/5_naive.jpg' width='435'/>
  <img src='results/5_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/6_naive.jpg' width='435'/>
  <img src='results/6_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/7_naive.jpg' width='435'/>
  <img src='results/7_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/8_naive.jpg' width='435'/>
  <img src='results/8_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/9_naive.jpg' width='435'/>
  <img src='results/9_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/10_naive.jpg' width='435'/>
  <img src='results/10_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/11_naive.jpg' width='435'/>
  <img src='results/11_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/12_naive.jpg' width='435'/>
  <img src='results/12_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/13_naive.jpg' width='435'/>
  <img src='results/13_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/14_naive.jpg' width='435'/>
  <img src='results/14_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/15_naive.jpg' width='435'/>
  <img src='results/15_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/16_naive.jpg' width='435'/>
  <img src='results/16_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/17_naive.jpg' width='435'/>
  <img src='results/17_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/18_naive.jpg' width='435'/>
  <img src='results/18_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/19_naive.jpg' width='435'/>
  <img src='results/19_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/20_naive.jpg' width='435'/>
  <img src='results/20_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/21_naive.jpg' width='435'/>
  <img src='results/21_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/22_naive.jpg' width='435'/>
  <img src='results/22_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/23_naive.jpg' width='435'/>
  <img src='results/23_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/24_naive.jpg' width='435'/>
  <img src='results/24_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/25_naive.jpg' width='435'/>
  <img src='results/25_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/26_naive.jpg' width='435'/>
  <img src='results/26_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/27_naive.jpg' width='435'/>
  <img src='results/27_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/28_naive.jpg' width='435'/>
  <img src='results/28_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/29_naive.jpg' width='435'/>
  <img src='results/29_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/30_naive.jpg' width='435'/>
  <img src='results/30_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/31_naive.jpg' width='435'/>
  <img src='results/31_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/32_naive.jpg' width='435'/>
  <img src='results/32_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/33_naive.jpg' width='435'/>
  <img src='results/33_final_res.png' width='435'/>
</p>
<p align='center'>
  <img src='data/34_naive.jpg' width='435'/>
  <img src='results/34_final_res.png' width='435'/>
</p>

