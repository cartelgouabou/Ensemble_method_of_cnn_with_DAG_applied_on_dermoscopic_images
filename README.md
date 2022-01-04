## Ensemble_method_of_cnn_with_DAG_applied_on_dermoscopic_images
_________________

Official implementation code of the paper [Ensemble Method of Convolutional Neural Networks with Directed Acyclic Graph Using Dermoscopic Images: Melanoma Detection Application](https://www.mdpi.com/1424-8220/21/12/3999) in Tensorflow.

### Dependency
The code is buil with following libraries
- Tensorflow 2.4
- Numpy
- Matlab R2020a
- GraphPad prism 5.03
- scikit-learn

### Dataset
- ISIC2018 [ISIC2018](https://challenge.isic-archive.com/data/). The original data will be preprocessed and split by `preprocessing.py`.

### Training
We provide several training examples with this repo:

- To train the HMLoss baseline on long-tailed imbalance with ratio of 100

```bash
python cifar_train.py --gpu 0 --imb_type exp --imb_factor 0.01 --loss_type CE --train_rule None
```


### Reference

If you find our paper and repo useful, please cite as

```
@article{foahom2021ensemble,
  title={Ensemble Method of Convolutional Neural Networks with Directed Acyclic Graph Using Dermoscopic Images: Melanoma Detection Application},
  author={Foahom Gouabou, Arthur Cartel and Damoiseaux, Jean-Luc and Monnier, Jilliana and Iguernaissi, Rabah and Moudafi, Abdellatif and Merad, Djamal},
  journal={Sensors},
  volume={21},
  number={12},
  pages={3999},
  year={2021},
  publisher={Multidisciplinary Digital Publishing Institute}
}
