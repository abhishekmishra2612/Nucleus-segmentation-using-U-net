# Nucleus-segmentation-using-U-net

## Overview :
Imagine speeding up research for almost every disease, from lung cancer and heart disease to rare disorders. The 2018 Data Science Bowl offers our most ambitious mission yet: create an algorithm to automate nucleus detection.

We’ve all seen people suffer from diseases like cancer, heart disease, chronic obstructive pulmonary disease, Alzheimer’s, and diabetes. Many have seen their loved ones pass away. Think how many lives would be transformed if cures came faster.

By automating nucleus detection, you could help unlock cures faster—from rare disorders to the common cold.
Identifying the cells’ nuclei is the starting point for most analyses because most of the human body’s 30 trillion cells contain a nucleus full of DNA, the genetic code that programs each cell. Identifying nuclei allows researchers to identify each individual cell in a sample, and by measuring how cells react to various treatments, the researcher can understand the underlying biological processes at work.
### Blog where i described the work: https://medium.com/@abhishekmishra_22309/detect-nuclei-semantic-segmentation-c8212cf69ef0
### Source of dataset: https://www.kaggle.com/c/data-science-bowl-2018/data
## Business Problem: 
   create a sementic segmentation model that can identify a range of nuclei across varied conditions. By observing patterns, Given a microscopic cell image contain various pattern of the nuclei and segments each nuclei.(It is Sementic segmentation problem).
### Performance metrics :
  The evaluation metrics for this sementic segmentation problem is mean Intersection over Union. The IoU of a proposed set of object pixels and a set of true object pixels is calculated as:
  ##                     IoU(A,B)=A∩B/A∪B.
  ### constraints :
   It not a low letency problem but the cost of error is very high because it is the medical problem prespective task where the cost of error is always high
   
 ## Steps :
 1.) Load the train(Images, masks) and test(Images,) and then extract the features from images and masks of train and test data into the numpy array so that we can preprocess the iamges and masks and manipulates it.
 
 2.) Then did data augmentation to increase the samples for training to overcome of overfitting problem. Data augmentation on both images and masks with the same seed value.
 
 3.) Built a U-net model with input shape=(128,128,3) and for output we get one mask image for a corresponding cell image.
 
 I got 0.7423 validation Mean_IoU that is reasonably good performance.
  
### Some predicted masks images:

#### for a training microscopic cell image : 
![Screenshot (109)](https://user-images.githubusercontent.com/41646536/86352383-5752c000-bc83-11ea-8b14-68ffe40ccfa5.png)

#### for some test microscopic cell image : 
![Screenshot (111)](https://user-images.githubusercontent.com/41646536/86352658-c16b6500-bc83-11ea-9593-96b5291e38b3.png)
