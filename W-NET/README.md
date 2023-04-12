Key Points
W-Net is a type of deep learning model designed for unsupervised image segmentation, which is gaining importance due to the high cost, time, and difficulty associated with obtaining image labeling in new domains..

The crux of this paper lies in
W-Net Architecure : The W-Net architecture is composed of two U-Net models that are concatenated together. The first U-Net model serves as an encoder, producing a segmentation of the input image. The second U-Net model is used as a decoder, reconstructing the original image from the segmentation produced by the encoder.
The U-Encoder in the W-Net architecture is responsible for generating image segmentations from unlabelled input images. 
On the other hand, the U-Decoder is responsible for reconstructing the original images from the segmentations produced by the U-Encoder.


The contraction path(Downsampling ) involves applying a 3x3 convolution without padding, followed by a ReLU activation and 2x2 max pooling with a stride of 2 to downsample the feature map. With each downsampling step, the number of feature channels doubles, which helps to capture context in a more concise feature map.

The expansion path then performs an upsampling of the feature map, followed by a 2x2 "up-convolution" that reduces the number of feature channels by half

Data augmentation: The authors advocate for the use of excessive data augmentation to improve the performance of the network.

Loss function: The paper proposes a modified dice loss function, which is designed to address class imbalance in the segmentation task.

Results: The authors evaluate the U-Net architecture on several biomedical segmentation tasks, including cell segmentation, optic disc segmentation, and liver segmentation. The U-Net architecture achieves state-of-the-art results on these tasks, outperforming other segmentation methods.

