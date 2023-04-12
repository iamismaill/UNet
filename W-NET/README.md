## Key Points

W-Net is a type of deep learning model designed for unsupervised image segmentation, which is gaining importance due to the high cost, time, and difficulty associated with obtaining image labeling in new domains..

### The crux of this paper lies in

* W-Net Architecure : The W-Net architecture is composed of two U-Net models that are concatenated together. The first U-Net model serves as an encoder, producing a segmentation of the input image. The second U-Net model is used as a decoder, reconstructing the original image from the segmentation produced by the encoder.
* The U-Encoder in the W-Net architecture is responsible for generating image segmentations from unlabelled input images. 

* On the other hand, the U-Decoder is responsible for reconstructing the original images from the segmentations produced by the U-Encoder.

* The W-Net architecture also includes a soft normalized cut loss function that simultaneously minimizes the total normalized disassociation between groups and maximizes the total normalized association within groups.

* The W-Net model used a soft version of the normalized cut (N cut) loss as its primary objective function. This loss function encouraged the model to group pixels together that were similar in color or texture while separating pixels that were dissimilar.
 
![W-net](https://user-images.githubusercontent.com/51711008/231480124-1be19b4c-b39e-4ad3-b7c6-f1989241a1df.png)
