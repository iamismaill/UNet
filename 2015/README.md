## Key Points 

The U-Net architecture is a modification of the Fully Convolutional Network that is designed for better segmentation in medical imaging. The architecture uses excessive data augmentation, including elastic deformations, to enable the network to learn invariance to such deformations without the need to see them in the annotated image corpus.

### The crux of this paper lies in 
* The U-Net paper proposes a convolutional neural network architecture for semantic segmentation in biomedical image analysis. Here are the key points of the paper:

* U-Net architecture: The U-Net architecture consists of a contracting path and an expansive path, with skip connections between them. The contracting path captures high-level context information through convolutional and pooling layers, while the expansive path enables precise localization through transposed convolutions.

* Data augmentation: The authors advocate for the use of excessive data augmentation to improve the performance of the network. 

* Loss function: The paper proposes a modified dice loss function, which is designed to address class imbalance in the segmentation task.

* Results: The authors evaluate the U-Net architecture on several biomedical segmentation tasks, including cell segmentation, optic disc segmentation, and liver segmentation. The U-Net architecture achieves state-of-the-art results on these tasks, outperforming other segmentation methods.

My Implementation ...

