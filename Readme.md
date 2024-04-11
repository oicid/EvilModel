# EvilModel

This is a lite version of [EvilModel](https://doi.org/10.1016/j.cose.2022.102807), which hides malware into neural network models without affecting their performances. In [EvilModel 2.0](https://doi.org/10.1016/j.cose.2022.102807), there are three methods to embed the malware into the models. The one with the least impact on model performance is "half substitution", which replaces two bytes of a parameter with malware bytes. This is the implementation of the "half substitution" in EvilModel. 

Note: this is not the full code of EvilModel. It's just a demo.

## Tips

`ImageNet` dataset is needed to test the performance of the models. Please download [ImageNet 2012](https://www.image-net.org/download.php) (`ILSVRC2012_img_val.tar` and `ILSVRC2012_devkit_t12.tar.gz`) and put them in the `Imagenet` dir.

`models` dir contains the offline pretrained models that saved from [PyTorch](https://github.com/pytorch/vision) repository. The model used in this demo is `ResNet50` (resnet50-19c8e357.pth). The offline models in EvilModel experiments are available at [Google Drive](https://drive.google.com/file/d/1bWu-2jBig-Lbo2KNC_uRnbVY0ABTjs55/view?usp=share_link).

`Malware` dir contains the samples we used in the experiments. We only use `Lazurus` in this demo. Full version of `Malware` is collected from [theZoo](https://github.com/ytisf/theZoo) and [InQuest](https://github.com/InQuest/malware-samples), and is available at [Google Drive](https://drive.google.com/file/d/15ivwxbQBadkXBgI8LGTyMWYQOrXMs1YP/view?usp=share_link) (unzip password: `malware`).

## Supplementaries

__Other implementations__

They're awesome :) 
[Implementation 1](https://github.com/gaborvecsei/Neural-Network-Steganography) (by [@Gábor Vecsei](https://www.gaborvecsei.com/)) [Implementation 2](https://github.com/fishjojo1/pyfltemb) [Implementation 3](https://hiddenlayer.com/research/weaponizing-machine-learning-models-with-ransomware/) 

[Slides](https://zw.ac.cn/files/EvilModel_presentation.pdf) at [ISCC 2021](https://iscc2021.unipi.gr/)

## Cite

EvilModel
```
@INPROCEEDINGS{EvilModel2021,
    author={Wang, Zhi and Liu, Chaoge and Cui, Xiang},
    booktitle={2021 IEEE Symposium on Computers and Communications (ISCC)}, 
    title={{EvilModel}: Hiding Malware Inside of Neural Network Models}, 
    year={2021},
    volume={},
    number={},
    pages={1-7},
    doi={10.1109/ISCC53001.2021.9631425}
}
```

EvilModel 2.0
```
@ARTICLE{evilmodel2,
    title = {{EvilModel} 2.0: Bringing Neural Network Models into Malware Attacks},
    author = {Wang, Zhi and Liu, Chaoge and Cui, Xiang and Yin, Jie and Wang, Xutong}
    journal = {Computers & Security},
    volume = {120},
    pages = {102807},
    year = {2022},
    issn = {0167-4048},
    doi = {https://doi.org/10.1016/j.cose.2022.102807},
}
```
