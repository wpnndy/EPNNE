# EPNNE
## Evolutionary Ensemble Learning for EEG-based Cross-Subject Emotion Recognition

This work is accepted by IEEE Journal of Biomedical and Health Informatics.

<div>
    </p>
    <a href="https://github.com/Audio-WestlakeU/FS-EEND/"><img src="https://img.shields.io/badge/Platform-Windows-lightgrey" alt="version"></a>
    <a href="https://github.com/Audio-WestlakeU/FS-EEND/"><img src="https://img.shields.io/badge/Python-3.8-orange" alt="version"></a>
</div>

[Paper :star_struck:](https://ieeexplore.ieee.org/document/10490105) **|** [Contact :kissing_heart:](zhanghz@sari.ac.cn)

# Introduction

Electroencephalogram (EEG) has been widely utilized in emotion recognition due to its high temporal resolution and reliability. However, the individual differences and non-stationary characteristics of EEG, along with the complexity and variability of emotions, pose challenges in generalizing emotion recognition models across subjects. In this paper, an end-to-end framework is proposed to improve the performance of cross-subject emotion recognition. A novel evolutionary programming (EP)-based optimization strategy with neural network (NN) as the base classifier termed NN ensemble with EP (EPNNE) is designed for cross-subject emotion recognition. The effectiveness of the proposed method is evaluated on the publicly available DEAP, FACED, SEED, and SEED-IV datasets. 

<div align="center">
<image src="/framework.png"  width="800" alt="Proposed end-to-end framework for cross-subject emotion recognition" />
</div>

# Performance
Please refer to the Experiments folder for more detailed results.

(2) Confusion Matrix: To gain a more detailed understanding of the recognition performance, we employed a confusion matrix to provide a comprehensive view of the results. The confusion matrix clearly displays the probability of each emotion being correctly recognized and the probability of being misclassified as other emotions.


<div align="center">
<image src="/conmax.png"  width="800" alt="Proposed end-to-end framework for cross-subject emotion recognition" />
</div>

# Citation

If you want to cite this paper:

```
@ARTICLE{10490105,
  author={Zhang, Hanzhong and Zuo, Tienyu and Chen, Zhiyang and Wang, Xin and Sun, Poly Z.H.},
  journal={IEEE Journal of Biomedical and Health Informatics}, 
  title={Evolutionary Ensemble Learning for EEG-based Cross-Subject Emotion Recognition}, 
  year={2024},
  volume={},
  number={},
  pages={1-10},
  keywords={Emotion recognition;Brain modeling;Electroencephalography;Feature extraction;Biological neural networks;Adaptation models;Data models;Emotion Recognition;Electroencephalogram;Cross-Subject Transfer Learning;Ensemble Learning},
  doi={10.1109/JBHI.2024.3384816}}
```
