# Thesis Semantic Image Segmentation on Satellite Imagery using UNets

This master thesis aims to perform semantic segmentation of buildings on satellite images from
the SpaceNet challenge 1 dataset using the U-Net architecture.
To enable a more focused use of feature-maps, soft attention mechanisms
are integrated into the U-Net and examined.
Furthermore, possibilities of transfer learning are investigated by
using convolutional neural networks pre-trained
on ImageNet as encoders for the U-Net.
Finally, the performance and robustness for the segmentation task is evaluated for both approaches.

## Prerequisites

It is assumed that you have [anaconda Python](https://www.anaconda.com/) installed. You can create a Python
environment with the required dependencies by following:

```
conda create -n thesis_env python=3.7
conda activate thesis_env
conda install numpy pandas rasterio shapely geopandas matplotlib imageio scikit-image
conda install pytorch torchvision torchaudio cudatoolkit=11.0 -c pytorch
conda install tifffile
```

If your CUDA versions differ please refer to [Start Locally | PyTorch](https://pytorch.org/get-started/locally/).

## Model weights

The model weights can be found at:

* [U-Net](https://drive.protonmail.com/urls/0K1DQWA7BW#FHqatMWKW81I)
* [Attention U-Net](https://drive.protonmail.com/urls/H0M2CM57ZR#omG2xLYB4R9R)
* [CBAM U-Net](https://drive.protonmail.com/urls/KQW02V5HTW#1re9Edplo6QY)
* [Residual Attention U-Net](https://drive.protonmail.com/urls/8PVP5JE2J4#JYg7IsbbOXK7)
* [scAG U-Net](https://drive.protonmail.com/urls/1P81WARY6C#Z51ijrV9bdg0)
* [DenseNet121 U-Net](https://drive.protonmail.com/urls/D5QT4C92YW#3DE25wzni9Ci)
* [MobileNetV2 U-Net](https://drive.protonmail.com/urls/TJW6F5THT8#MtqNAn0k1YxZ)
* [ResNet34 U-Net](https://drive.protonmail.com/urls/6T6354SJZC#EP8B6RmRojVA)
* [VGG11 U-Net](https://drive.protonmail.com/urls/8K3F124Y9C#dc7c0LcjCfri)

## Authors

* [Philip Rinkwitz](https://github.com/rinkwitz)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
The helper methods in ```Utils/SolarisHelpers.py``` are taken from the [Solaris](https://github.com/CosmiQ/solaris) project
that is licensed under the [Apache-2.0 License](https://github.com/CosmiQ/solaris/blob/master/LICENSE.txt). 
Please refer to that license if you plan on reusing that code.

[comment]: <> (<p align="center">)

[comment]: <> (<img src="/img/rml_country.jpg" alt="rml country" width="600">)

[comment]: <> (<img src="/img/table_country.png" alt="table country" width="415">)

[comment]: <> (</p>)


[comment]: <> (## Acknowledgements:)

[comment]: <> (The formulas of this README were create using:)

[comment]: <> (* [Codecogs online Latex editor]&#40;https://www.codecogs.com/latex/eqneditor.php&#41;)
