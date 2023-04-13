## Key Points
* Colonoscopy is a medical procedure performed to detect the anomalies in the colon and rectum, The physicians find it very challenging to diagnose small polyps in colonoscopy video
* 
* In this work UNET architecture with spatial attention layer is proposed to improve the precision of segmenting polyp regions in colonoscopy video. The CNN models proposed in the literature for polyp segmentation are basically trained using common loss functions such as dice and binary cross entropy loss.

* In this work UNET architecture with spatial attention layer is proposed to improve the precision of segmenting polyp regions in colonoscopy video. The CNN models proposed in the literature for polyp segmentation are basically trained using common loss functions such as dice and binary cross entropy loss

* The encoder network consists of a series of con layers with batch normalization and  Relu activation followed by Max pooling layers.

* The decoder network consists of series of transposed conv layers that up-samples features back to the original image size followed by modified skip connections that concatenate the features from the corresponding encoder layer through SAL (Spatial attention layer) 

* SAL is used to generate the spatial relationship between the features produced at each stage of the encoder, in order to extract spatial information from low-level features
*
* In Image Segmentation , the choice of loss functions is crucial in training deep learning models 

* In the proposed work , UNet and UNet with modified skip connections is trained with various loss functions which are binary cross entropy (BCE) , Dice Loss and Mean Squared Error - however these loss functions didn’t effectively segment small polyps as they weigh false positives and false negatives equally resulting in high precision and low recall So they propose using Focal Tversky Loss(FTL) to balance the detection of false negatives and false positives



![updatedone](https://user-images.githubusercontent.com/51711008/231824957-f8efb5dd-0e54-42c9-85c3-bb4413a04f21.png)
