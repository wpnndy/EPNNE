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

(1) SEED Results 

|  | sub1 | sub2 | sub3 | sub4 | sub5 |  sub6 |  sub7 |  sub8 |  sub9 |  sub10 |  sub11 |  sub12 |  sub13 |  sub14 |  sub15 | Avg | 
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
TCA | 0.723 | 0.644 | 0.678 | 0.651 | 0.641 | 0.750 | 0.678 | 0.713 | 0.746 | 0.690 | 0.687 | 0.608 | 0.674 | 0.709 | 0.652 | 0.684
JDA | 0.673 | 0.764 |  0.732 | 0.680 | 0.665 | 0.729 | 0.678 | 0.806 | 0.846 | 0.819 | 0.731 | 0.644 | 0.676 | 0.760 | 0.819 | 0.735
| FSTSL  | 0.759 | 0.803  | 0.838 | 0.811 | 0.841 | 0.708 | 0.795 | 0.757 | 0.806 | 0.780 | 0.899 | 0.691 | 0.742 | 0.776 | 0.915 | 0.795
MIDA| 0.768 | 0.775 | 0.765 | 0.848 | 0.742 | 0.652 | 0.758 | 0.729 | 0.742 | 0.770 | 0.821 | 0.606 | 0.717 | 0.743 | 0.742 | 0.746
MEKT| 0.785 | 0.789 | 0.765 | 0.847 | 0.881 | 0.835 | 0.817 | 0.840 | 0.879 | 0.764 | 0.932 | 0.791 | 0.737 | 0.786 | 0.718 | 0.811
LA| 0.689 | 0.691 | 0.680 | 0.832 | 0.673 | 0.759 | 0.490 | 0.542 | 0.801 | 0.786 | 0.740 | 0.761 | 0.777 | 0.643 | 0.648 | 0.701
JTSR| 0.843 | 0.878 | 0.762 | 0.881 | 0.871 | 0.814 | 0.835 | 0.861 | 0.922 | 0.779 | 0.923 | 0.832 | 0.823 | 0.795 | 0.870 | 0.847 |
DS3TL| 0.825 | 0.753 | 0.795 | 0.956 | 0.854 | 0.829 | 0.844 | 0.746 | 0.763 | 0.836 | 0.883 | 0.677 | 0.777 | 0.885 | 0.828 | 0.817 |
EPNNE| 0.875 | 0.825 | 0.931 | 0.933 | 0.904 | 0.930 | 0.879 | 0.894 | 0.907 | 0.945 | 0.915 | 0.881 | 0.843 | 0.827 | 0.873 | 0.891 |

|  | sub2 | sub3 | sub4 | sub5 |  sub6 |  sub7 |  sub8 |  sub9 |  sub10 |  sub11 |  sub12 |  sub13 |  sub14 |  sub15 | Avg | 
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | :----: | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
TCA | 0.680 | 0.618 | 0.704 | 0.648 | 0.667 | 0.629 | 0.625 | 0.889 | 0.667 | 0.728 | 0.585 | 0.690 | 0.710 | 0.561 | 0.672 | 
JDA | 0.665 | 0.633 | 0.727 | 0.633 | 0.727 | 0.671 | 0.669 | 0.898 | 0.734 | 0.818 | 0.647 | 0.659 | 0.792 | 0.717 | 0.714 | 
| FSTSL  | 0.662 | 0.604 | 0.624 | 0.775 | 0.699 | 0.725 | 0.673 | 0.718 | 0.728 | 0.830 | 0.614 | 0.810 | 0.792 | 0.907 | 0.726 | 
MIDA| 0.701 | 0.608 | 0.808 | 0.562 | 0.636 | 0.712 | 0.708 | 0.896 | 0.730 | 0.830 | 0.690 | 0.606 | 0.771 | 0.723 | 0.713 | 
MEKT| 0.659 | 0.607 | 0.705 | 0.728 | 0.775 | 0.761 | 0.656 | 0.798 | 0.677 | 0.823 | 0.732 | 0.607 | 0.686 | 0.652 | 0.705 | 
LA| 0.669 | 0.683 | 0.702 | 0.691 | 0.842 | 0.609 | 0.546 | 0.807 | 0.707 | 0.784 | 0.752 | 0.773 | 0.644 | 0.406 | 0.687 | 
JTSR| 0.706 | 0.743 | 0.814 | 0.740 | 0.729 | 0.765 | 0.772 | 0.779 | 0.744 | 0.802 | 0.766 | 0.719 | 0.746 | 0.770 | 0.757 | 
CORAL| 0.475 | 0.583 | 0.452 | 0.547 | 0.584 | 0.543 | 0.619 | 0.586 | 0.572 | 0.576 | 0.473 | 0.558 | 0.510 | 0.705 | 0.556 | 
MEDA| 0.638 | 0.569 | 0.551 | 0.630 | 0.650 | 0.606 | 0.710 | 0.668 | 0.664 | 0.671 | 0.501 | 0.619 | 0.638 | 0.755 | 0.634 | 
CSDS| 0.687 | 0.590 | 0.576 | 0.654 | 0.693 | 0.668 | 0.719 | 0.686 | 0.658 | 0.677 | 0.523 | 0.636 | 0.642 | 0.853 | 0.661 | 
EPNNE| 0.759 | 0.763 | 0.816 | 0.834 | 0.897 | 0.803 | 0.819 | 0.817 | 0.830 | 0.864 | 0.792 | 0.784 | 0.814 | 0.794 | 0.813 | 

(2) SEED-IV Results

|Session 1   | sub2 | sub3 | sub4 | sub5 |  sub6 |  sub7 |  sub8 |  sub9 |  sub10 |  sub11 |  sub12 |  sub13 |  sub14 |  sub15 | Avg | 
| :----: | :----: | :----: | :----: | :----: | :----: | :----: | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
GFK | 0.627 | 0.560 | 0.443 | 0.253 | 0.336 | 0.488 | 0.507 | 0.535 | 0.517 | 0.499 | 0.313 | 0.438 | 0.404 | 0.316 | 0.446 
TCA | 0.475 | 0.480 | 0.663 | 0.338 | 0.387 | 0.598 | 0.433 | 0.460 | 0.472 | 0.450 | 0.332 | 0.525 | 0.505 | 0.371 | 0.464
JDA | 0.578 | 0.647 | 0.682 | 0.485 | 0.515 | 0.701 | 0.654 | 0.648 | 0.656 | 0.519 | 0.542 | 0.629 | 0.555 | 0.691 | 0.608
MIDA | 0.676 | 0.584 | 0.447 | 0.465 | 0.478 | 0.549 | 0.663 | 0.533 | 0.638 | 0.593 | 0.591 | 0.506 | 0.439 | 0.466 | 0.551
DGCNN | 0.546 | 0.574 | 0.589 | 0.492 | 0.404 | 0.481 | 0.511 | 0.629 | 0.426 | 0.510 | 0.559 | 0.522 | 0.532 | 0.538 | 0.522
LRS | 0.491 | 0.392 | 0.428 | 0.326 | 0.213 | 0.426 | 0.475 | 0.432 | 0.467 | 0.424 | 0.633 | 0.334 | 0.408 | 0.337 | 0.413 
JAGP | 0.742 | 0.729 | 0.707 | 0.819 | 0.693 | 0.669 | 0.679 | 0.844 | 0.769 | 0.693 | 0.747 | 0.701 | 0.613 | 0.820 | 0.730
FSTSL | 0.602 | 0.582 | 0.607 | 0.512 | 0.460 | 0.512 | 0.424 | 0.618 | 0.542 | 0.485 | 0.481 | 0.501 | 0.498 | 0.561 | 0.528
MEKT | 0.535 | 0.725 | 0.596 | 0.703 | 0.506 | 0.668 | 0.626 | 0.631 | 0.607 | 0.602 | 0.675 | 0.683 | 0.544 | 0.517 | 0.616
LA | 0.655 | 0.666 | 0.654 | 0.689 | 0.591 | 0.705 | 0.639 | 0.643 | 0.653 | 0.661 | 0.744 | 0.655 | 0.654 | 0.607 | 0.658
JTSR | 0.749 | 0.719 | 0.787 | 0.742 | 0.679 | 0.750 | 0.733 | 0.855 | 0.729 | 0.747 | 0.756 | 0.683 | 0.694 | 0.729 | 0.739
EPNNE | 0.819 | 0.792 | 0.828 | 0.770 | 0.702 | 0.714 | 0.752 | 0.809 | 0.793 | 0.764 | 0.766 | 0.796 | 0.807 | 0.791 | 0.779 

(3) Confusion Matrix: To gain a more detailed understanding of the recognition performance, we employed a confusion matrix to provide a comprehensive view of the results. The confusion matrix clearly displays the probability of each emotion being correctly recognized and the probability of being misclassified as other emotions.


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
