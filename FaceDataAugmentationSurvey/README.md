**[Medium Article](https://link.medium.com/gBsAnKEEw6)**

**[Paper](https://arxiv.org/pdf/1904.11685.pdf)**

## Abstract
The above survey paper is written by three individuals working at a startup named CloudMinds which offers a PaaS
providing out of the box functionality for robot systems performing various tasks. 

## Section I: Intro
In this paper, various existing frameworks for face data augmentation are reviewed with a strong emphasis on GANs
which have been reognized as more powerful and effective than traditional tools. Additionally, various evaluation
metrics for looking at the quality of augmentation are discussed. Lastly, some important challenges in the
task of face data augmentation are pointed out as well. 

## Section II: Related Works

## Section III: Augmentation Types
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
  
## Section IV: Transformation Methods
Dives into the high level 2D geometry based facial augmentation methods and the architecture of GANs used to generate augmentation features listed in section III.
1. Basic Image Processing
2. Model-based transformation
3. Realism Enhancement
4. Generative-based Transformation
5. Agumented Reality

## Section V. Evaluation metrics
For qualitative evaluation, the authors directly present the readers or interviewers
with generated images and let them judge the quality. The
quantitative evaluation provides quantifiable and explicit results. Most
of the time, both qualitative and quantitative methods are
employed together to provide adequate information for the
evaluation, and suitable evaluation metrics should be applied
since face data augmentation includes different transformation
types with different purpose.

## Section VI. Challenges and Opportunities
1. Identity Preserving
2. Disentangled representation -- being able to point apart the augmented vs real data.
3. Unsupervised Augmentation
4. GAN improvements

## Section VII. Discussion
Talks about accomplishments vs. challenges and potential paths forward

## Section VIII. Conclusion
Closing remarks
