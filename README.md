










## DetectorWithFocus
Created by [Yonghyun Kim](http://imlab.postech.ac.kr/members.htm) and [Daijin Kim](http://imlab.postech.ac.kr/members_d.htm) at [POSTECH IM Lab](http://imlab.postech.ac.kr)

### Overview

An image pyramid can extend many object detection algorithms to solve detection on multiple scales. However, interpolation during the resampling process of an image pyramid causes gradient variation, which is the difference of the gradients between the original image and the scaled images. Our key insight is that the increased variance of gradients makes the classifiers have difficulty in correctly assigning categories. We prove the existence of the gradient variation by formulating the ratio of gradient expectations between an original image and scaled images, then propose a simple and novel gradient normalization method to eliminate the effect of this variation. The proposed normalization method reduce the variance in an image pyramid and allow the classifier to focus on a smaller coverage. We show the improvement in three different visual recognition problems: pedestrian detection, pose estimation, and object detection. The method is generally applicable to many vision algorithms based on an image pyramid with gradients.


## Citation
If you're using this code in a publication, please cite our papers.

```
  @inproceedings{ykim2017detector,
    title={DETECTOR WITH FOCUS: NORMALIZING GRADIENT IN IMAGE PYRAMID},
    author={Yonghyun Kim, Bongnam Kang and Daijin Kim},
    booktitle={IEEE International Conference on Image Processing (ICIP)},
    year={2017},
    organization={IEEE}
  } 
'''

### Performance

We conduct the experiments in object detection with three applications: pedestrian detection, pose estimation, and object detection.

### Overall
We propose ### Overalla simple and novel gradient normalization method by analyzing the gradient variation in the viewpoint of the classifier.
The proposed method defines the original image as reference, and normalizes gradients from other resampled images to the reference image. 
The normalized gradient, which is similar to the gradients of original images, reduces the variance, and increases the performance of the classifiers with negligible increase in computing time.
We show the effectiveness of the gradient normalization in object detection with three applications: pedestrian detection, pose estimation, and object detection.

### Related Papers

Yonghyun Kim, Bong-Nam Kang, Daijin Kim, "DETECTOR WITH FOCUS: NORMALIZING GRADIENT IN IMAGE PYRAMID," 2017  IEEE International Conference on Image Processing (ICIP) 2017.



### Acknowledgements

This work was supported by Institute for Information & communications Technology Promotion (IITP) grant funded by the Korea government (MSIP)(2014-0-00059, Development of Predictive Visual Intelligence Technology), MSIP (Ministry of Science, ICT and Future Planning), Korea, under the ICT Consilience Creative Program (IITP-R0346-16-1007) supervised by the IITP, and MSIP(Ministry of Science, ICT and Future Planning), Korea, under the ITRC (Information Technology Research Center) support program (IITP-2017-2016-0-00464) supervised by the IITP.
