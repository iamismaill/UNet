## Key Points 

The U-Net architecture is a modification of the Fully Convolutional Network that is designed for better segmentation in medical imaging. 

### The crux of this paper lies in 
* U-Net architecture: The U-Net architecture consists of a contracting path(downsampling) and an expansive path (upsampling), with skip connections between them. The contracting path captures high-level context information through convolutional and pooling layers, while the expansive path enables precise localization through transposed convolutions.

* The contraction path(Downsampling ) involves applying a 3x3 convolution without padding, followed by a ReLU activation and 2x2 max pooling with a stride 
of 2 to downsample the feature map. With each downsampling step, the number of feature channels doubles, which helps to capture context in a more concise feature map.

* The expansion path then performs an upsampling of the feature map, followed by a 2x2 "up-convolution" that reduces the number of feature channels by half

* Data augmentation: The authors advocate for the use of excessive data augmentation to improve the performance of the network. 

* Loss function: The paper proposes a modified dice loss function, which is designed to address class imbalance in the segmentation task.

* Results: The authors evaluate the U-Net architecture on several biomedical segmentation tasks, including cell segmentation, optic disc segmentation, and liver segmentation. The U-Net architecture achieves state-of-the-art results on these tasks, outperforming other segmentation methods.

My Implementation ...

