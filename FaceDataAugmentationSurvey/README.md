[Link to Paper](https://arxiv.org/pdf/1904.11685.pdf)

# Abstract
The above survey paper is written by three individuals working at a startup named CloudMinds which offers a PaaS
providing out of the box functionality for robot systems performing various tasks. 

In this paper, various existing frameworks for face data augmentation are reviewed with a strong emphasis on GANs
which have been reognized as more powerful and effective than traditional tools. Additionally, various evaluation
metrics for looking at the quality of augmentation are discussed. Lastly, some important challenges in the
task of face data augmentation are pointed out as well. 

Section III: Augmentation Types
There are 3 main areas of facial transofrmations: generic, component and attribute. 
* Generic 
  * Geometric - rotations, twisting and turning
  * Photomeretric - playing with RGB channel settings
* Component Transformation -> Utilizes GANs heavily
  * Hairstyle
  * Makeup
  * Accessory 
* Attribute
  * Pose
  * Expression
  * Age
  
Section IV: Transformation Methods
Dives into the high level 2D geometry based facial augmentation methods and the architecture of GANs used to generate augmentation features listed in section III.
1. Basic Image Processing
2. Model-based transformation
3. Realism Enhancement
4. Generative-based Transformation
5. Agumented Reality

Section V. Evaluation metrics

Section VI. Challenges and Opportunities

Section VII. Discussion

Section VIII. Conclusion
