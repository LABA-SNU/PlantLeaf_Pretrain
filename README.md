# PlantLeaf Pretrained Model
By Yunseok Han, Woosang Jeon, Sanghyeok Choi, Kyuseok Yang, Taehyeong Kim*

> Code will be available.

## Introduction
The agricultural sector still experiences a notable gap in foundational research on models tailored for its unique needs, particularly in addressing the diverse and complex challenges of data variability and environmental conditions inherent to agricultural applications. 
To bridge this gap, this study introduces **a deep learning-based vision foundation model for agriculture, specifically pretrained on extensive unlabeled plant leaf datasets using self-supervised learning methods like BYOL.**

<p align="center">
  <img src="./imgs/PlantLeaf_intro.png" width="600"/>
</p>

## Results ( with ResNet-50 )
|            Method            |          PVD          |     Pepper_chilli     |         Tomato        |        Lettuce        |
|:----------------------------:|:---------------------:|:---------------------:|:---------------------:|:---------------------:|
| Linear Evaluation :          |                       |                       |                       |                       |
| PlantLeaf Pretrained (Ours ) | **0.922 $\pm$ 0.001** |   0.826 $\pm$ 0.005   | **0.912 $\pm$ 0.002** | **0.625 $\pm$ 0.001** |
| ImageNet Pretrained          |   0.901 $\pm$ 0.002   | **0.854 $\pm$ 0.014** |   0.879 $\pm$ 0.011   |   0.521 $\pm$ 0.080   |
| Fine-tuned :                 |                       |                       |                       |                       |
| PlantLeaf Pretrained (Ours ) | **0.961 $\pm$ 0.003** | **0.939 $\pm$ 0.024** | **0.954 $\pm$ 0.013** | **0.848 $\pm$ 0.013** |
| ImageNet Pretrained          |   0.833 $\pm$ 0.008   |   0.729 $\pm$ 0.038   |   0.810 $\pm$ 0.018   |   0.356 $\pm$ 0.070   |
| Random init                  |   0.833 $\pm$ 0.008   |   0.833 $\pm$ 0.008   |   0.833 $\pm$ 0.008   |   0.833 $\pm$ 0.008   |

