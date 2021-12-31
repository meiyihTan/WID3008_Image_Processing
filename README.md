# WID3008 Image Processing Assignment - Face recognition with medical masks

## Objectives
1.	To recognize the identity of a masked individual.
2.	To evaluate the accuracy of the facial recognition net.

## Pipeline with training face recognition
The whole pipeline code for training with detailed description provided in google [colab notebook](https://colab.research.google.com/drive/1zqF0Zt71xhiP-2u25SzkDmc5CMdx4t1b?usp=sharing).

## Test medical masks augmentations
You can also test masked faces pipeline from this [colab notebook](https://colab.research.google.com/drive/1CCleAFWFaD_8F3dTWJeCrCb_Wamrmoe1?usp=sharing)

## To overcome
Identification systems which is we use for unlocking our devices have struggled with medical masks appearing on human faces.



## Solution
We will show and build system with the most modern state-of-the-art methods  possible to solve the task of face recognition with medical masks. 
In order to do that, we will make such augmentations that transform our initial training dataset into persons wearing medical masks.

![Trump](https://cdn-images-1.medium.com/max/1200/1*qFYQo4nqwc-wE_EseswvqA.png)

## Process of facial keypoints extraction
![Keypoints](https://drive.google.com/uc?export=view&id=1W_lPnFr3VuCyrSEBSJOnosiGPUzjSY4I)

## Triangulation process
![Triangulation](https://cdn-images-1.medium.com/max/1200/1*-KyFG7mHQnh9vdqkkpxyDA.png)

## Medical mask matching
![Mask](https://drive.google.com/uc?export=view&id=1lWUSRfauRNkJ1F71z1xP7lKl5DsUZOcM)

## Situation with the face rotation

Proposed solution also handles the situation with the face rotation, as medical masks database is stored in json with the calculated parameter of rotation, which allow us to match images with face rotation for only with those masks that are falling in concrete interval of rotation for given face.

![Rotation](https://cdn-images-1.medium.com/max/1200/1*p0wp1UTrM5Wj3RsgDpZ9vg.png)

## System Design
![Rotation](https://drive.google.com/uc?export=view&id=16LIqe2cSkWBNJWgoTONaqxx_ivQp8ZMs)

## ArcFace

Process of training a DCNN for face recognition supervised by the ArcFace loss

![ArcFace](https://cdn-images-1.medium.com/max/2560/1*T3wkuUKIqMunwfOoi5_kGg.png)

## Results
We were able to achieve 58 percents accuracy with **custom metric** on test dataset. The ability to show impressive results for such limited training time proves that pipeline is able to solve face recognition with medical masks task.

![Results](https://cdn-images-1.medium.com/max/1200/1*f7aMUHEvVB9WGIIyf8NtXQ.png)

## Acknowledgments
This repository contains the source code  borrows from the [**article**](https://broutonlab.com/blog/how-facial-recognition-works-with-face-masks) on Face recognition with medical masks by [Alexey Kovalenko](https://github.com/AlexeySrus) and [Artem Poltavskiy](https://github.com/poltavski)
