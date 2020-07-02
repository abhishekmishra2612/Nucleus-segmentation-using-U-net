# Nucleus-segmentation-using-U-net

## Overview :
Imagine speeding up research for almost every disease, from lung cancer and heart disease to rare disorders. The 2018 Data Science Bowl offers our most ambitious mission yet: create an algorithm to automate nucleus detection.

We’ve all seen people suffer from diseases like cancer, heart disease, chronic obstructive pulmonary disease, Alzheimer’s, and diabetes. Many have seen their loved ones pass away. Think how many lives would be transformed if cures came faster.

By automating nucleus detection, you could help unlock cures faster—from rare disorders to the common cold.
Identifying the cells’ nuclei is the starting point for most analyses because most of the human body’s 30 trillion cells contain a nucleus full of DNA, the genetic code that programs each cell. Identifying nuclei allows researchers to identify each individual cell in a sample, and by measuring how cells react to various treatments, the researcher can understand the underlying biological processes at work.
### Source of dataset: https://www.kaggle.com/c/data-science-bowl-2018/data
## Business Problem: 
   create a sementic segmentation model that can identify a range of nuclei across varied conditions. By observing patterns, Given a microscopic cell image contain various pattern of the nuclei and segments each nuclei.(It is Sementic segmentation problem).
### Performance metrics :
  The evaluation metrics for this sementic segmentation problem is mean Intersection over Union. The IoU of a proposed set of object pixels and a set of true object pixels is calculated as:
  ##                     IoU(A,B)=A∩B/A∪B.
  ### constraints :
   It not a low letency problem but the cost of error is very high because it is the medical problem prespective task where the cost of error is always high
   
   
