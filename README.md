# **Pinwheel-shaped Convolution and Scale-based Dynamic Loss for Infrared Small Target Detection**
--------

### In this paper, we proposed a plug-and-play PConv module, leveraging the Gaussian distribution characteristics of IRST to achieve an efficient, larger receptive field with minimal parameters. We also introduced a simple yet effective SD loss function to address IoU fluctuation issues with labels. Furthermore, we introduced the SIRST-UAVB dataset, a large-scale and challenging benchmark with detailed annotations. Our contributions can be summarized as follows:

  (1) Based on the Gaussian spatial distribution of IRST, we propose a novel plug-and-play convolutional module, PConv, which enhances CNNs' ability to analyze bottom-layer features of IRST.
  
  (2) We introduce SD loss, which dynamically adjusts the impact coefficients of Scale loss and Location loss, improving the neural network’s regression capability and detection performance across targets of varying scales.
  
  (3) We construct SIRST-UAVB, the largest publicly dataset for real IRSTDS, encompassing comprehensive spatial domain challenges.
  
  (4) We apply PConv and SD Loss to both BBox and mask label formats in IRSTDS methods, validating their effectiveness and generalization across public datasets and our own. Experimental results demonstrate significant and consistent performance enhancements.

--------
## ___step 1.  DATA Preparation___   

  *Download the datasets and put them to './data'.*
  
  [IRSTD-1K](URL 'https://github.com/RuiZhang97/ISNet')  
  [IRSTD-1K][BBOX_labels](dir ./data/IRSTD-1K-labels/labels)  

  [SIRST-UAVB]  ![Github stars](https://img.shields.io/badge/License-MIT-blue)    
  [google](URL '[https://drive.google.com/file/d/1hANdynk5C3fUQ1z2CqLRhAqUAfEsaWq8/view?usp=drive_link](https://drive.google.com/file/d/1hANdynk5C3fUQ1z2CqLRhAqUAfEsaWq8/view?usp=sharing)')  
  [baidu](URL 'https://pan.baidu.com/s/1FIg6BU8jlZogEQYWx_-ubQ?pwd=0558')  (Extraction code：'0558'))


## ___step 2. Selection algorithm___

  *Download CNN-based IRSTD algorithms that need to be improved*  

  Such as [yolov8n-p2](URL 'https://github.com/ultralytics/ultralytics.git') or [MSHNet](URL 'https://github.com/Lliu666/MSHNet').

  *PConv and SD loss are used to replace the corresponding parts of the original algorithm.*


##
* The SD loss code is highly borrowed from [CIoU loss](https://github.com/Zzh-tju/CIoU) and [SLS loss](URL 'https://github.com/Lliu666/MSHNet'). Thanks to Zhaohui Zheng and Qiankun Liu.
  



    
  
 



