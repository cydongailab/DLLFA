<div align="center">
<h2> Dual-Level Language-Frames Attention for Text-Video Retrieval </h2>

[Chuang Dong](), [Wei Li](http://faculty.neu.edu.cn/liwei1/zh_CN/index.htm), [Gang Li](),  [Mengtian Huang](), [Zhengqi Huang](), [Zhaolu Feng](), [Jinzhu Yang]()

[Northeastern University](https://www.neu.edu.cn/)


</div>

# DLLFA

## Introduction

This repository contains the offical  implementation of DLLFA, which can effectively improve the accuracy of video-text retrieval. Our code will be released soon!


## Motivation
The key to aggregating multi-frame image features into video feature: Temporal order/The relevance of the frame to the overall meaning of the video 
<div align=center>
<img width="500" alt="image" src="img/time.png">


<img width="500" alt="image" src="img/relevance.png">

</div>

## DLLFA Modal
<img  alt="image" src="img/DLLFA.png">


## Requirement

```shell
pip install -r requirements.txt
pip install torch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2
```

## Download CLIP Model 

```shell
wget https://openaipublic.azureedge.net/clip/models/40d365715913c9da98579312b702a82c18be219cc2a73407c4526f58eba950af/ViT-B-32.pt
wget https://openaipublic.azureedge.net/clip/models/5806e77cd80f8b59890b7e101eabd078d9fb84e6937f9e85e4ecb61988df416f/ViT-B-16.pt
```

## Datasets

| Datasets   | Link                                                         |
| ---------- | ------------------------------------------------------------ |
| MSR-VTT-9K | http://ms-multimedia-challenge.com/2017/dataset              |
| MSR-VTT-7K | http://ms-multimedia-challenge.com/2017/dataset              |
| LSMDC      | [Large Scale Movie Description Challenge - Download (google.com)](https://sites.google.com/site/describingmovies/download) |
| VATEX      | https://eric-xw.github.io/vatex-website/download.html        |



## Results

<div align=center>
<img  alt="image" src="img/msrvtt.png">
<img  alt="image" src="img/vatex.png">
<img  alt="image" src="img/lsmdc.png">
</div>


##  Citation

```bibtex
@article{DLLFA,
  title={Dual-Level Language-Frames Attention for Text-Video Retrieval},
  author={Dong, Chuang and Li, Wei and Li, Gang},
  journal={},
  year={2023}
}
```

## Acknowledgment
Our implementation is mainly based on the following codebases. We are sincerely grateful for their work.
- [Cap4Video](https://github.com/whwu95/Cap4Video): Cap4Video: What Can Auxiliary Captions Do for Text-Video Retrieval?
- [CLIP4Clip](https://github.com/ArrowLuo/CLIP4Clip): An Empirical Study of CLIP for End to End Video Clip Retrieval
- [ATP](https://github.com/StanfordVL/atp-video-language): Revisiting the "Video" in Video-Language Understanding
```
