# EV-Action: Electromyography Vision Multi-Modal Action Dataset
This repository contains code for our IEEE International Conference on Automatic Face and Gesture Recognition (FG) paper: [EV-Action: Electromyography Vision Multi-Modal Action Dataset](https://arxiv.org/abs/1904.12602).

## Our paper
### Introduction

Multi-label learning (MLL) solves the problem that one single sample corresponds to multiple labels. It is a challenging task due to the long-tail label distribution and the sophisticated label relations. Semi-supervised MLL methods utilize a small-scale labeled samples and large-scale unlabeled samples to enhance the performance. However, these approaches mainly focus on exploring the data distribution in feature space while ignoring mining the label relation inside of each instance. 

<div align="center">
    <img src="presentation/concept.png", width="450">
</div>

We proposed a Dual Relation Semi-supervised Multi-label Learning (DRML) approach which jointly explores the feature distribution and the label relation simultaneously. A dual-classifier domain adaptation strategy is proposed to align features while generating pseudo labels to improve learning performance. A relation network is proposed to explore the relation knowledge. As a result, DRML effectively explores the feature-label and label-label relations in both labeled and unlabeled samples. It is an end-to-end model without any extra knowledge. Extensive experiments illustrate the effectiveness and efficiency of our method.

### Our model
<div align="center">
    <img src="presentation/model.png", width="1000">
</div>

DRML includes a novel domain adaptation co-training strategy and a label relation mining module in semi-supervised fashion. It explores both the instance similarity in feature space and the label-label relation in label space simultaneously. Specifically, deploy a two-classifier domain adaptation strategy to align the feature distribution in a latent space. Moreover, it further provides the pseudo label of unlabeled samples to enhance the training performance. Furthermore, a relation network is proposed to utilize the predictions from the two classifiers to learn the label relations. All modules are simultaneously optimized in an end-to-end manner to achieve the highest performance. The major contributions of our work are briefly listed as follows:

* A two-classifier domain adaptation co-training strategy is proposed. It aligns the labeled and unlabeled samples in feature space to improve model accuracy and robustness.
* A label assignment strategy is proposed to generate pseudo labels to the unlabeled data. The assigned samples are further utilized in the training process.
* A graph-based relation network is proposed to learn the label relations for both labeled and unlabeled samples.


## Running the code
The dataset and code will be available soon. Feel free to send email if you have any questions!

## Authors
Welcome to send us Emails if you have any questions about the code and our work :-)
* **Lichen Wang** [Website](https://sites.google.com/site/lichenwang123/)
* **Bin Sun**
* **Joseph Robinson** [Website](https://www.jrobsvision.com/)
* **Taotao Jing** [Website](https://scholar.google.com/citations?user=cvrjwJIAAAAJ&hl=en)
* **Yun Raymond Fu** [Website](http://www1.ece.neu.edu/~yunfu/)

## Citation
```
@article{EVaction_lichen,
  title={EV-Action: Electromyography-Vision Multi-Modal Action Dataset},
  author={Wang, Lichen and Sun, Bin and Robinson, Joseph and Jing, Taotao and Fu, Yun},
  journal={arXiv preprint arXiv:1904.12602},
  year={2019}
}
```


