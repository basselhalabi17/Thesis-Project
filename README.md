# FinalThesisSubmission

The repo includes all the notebooks and codebase we used in implementing all steps of our research in building a model to convert signs from the American sign language (ASL) to text, and the other way around from Audio to Sign 

# Dataset Link

https://drive.google.com/drive/folders/1jAg9pGxOlT5Bsqy9686LPSC0zh3jMNX5?usp=sharing


# Repo Contents 

## Resizing and Normalization 

In this notebook, we performed the dimensions normalization as well as frames standardization among all of our dataset in order to be able to extract keypoints from the videos 

## Augmentation 

In this notebook, we implemented the Augmentations needed to increase the mean of our classes from 22 to 129 videos per class. 

## Extracting Data Points

In this notebook, we implemented our keypoints extracation from our dataset, in which every video is segemented into 30 frames, and we generate a npy file for each frame that contains the extracted keypoints for the corresponding frame

## Model

Our Thesis Cornerstone. In this notebook, we designed and implemented our model. The notebook holds training and testing statistics for the latest model (100 Words) we trained. 

## Testing Realtime

In this notebook, we implemented our camera detection module that can detect keypoints for a signer using a camera. Afterwards, the keypoints are passed to our model to provide the top 5 predictions. We used our 80 Words model in this module, as among all of our experiments it holded realtivaly high accuarcy to number of classes ratio 

## Audio to Sign Pipeline 

In this notebook, we implemented our second pipeline, utilizing the NLPTK and our Signs Database 
