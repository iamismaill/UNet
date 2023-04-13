
## Key Points
* Anomaly detection in surveillance video is of great significance for public safety. Deep autoencoder has been widely used in anomaly detection. Because of its good generalization ability, sometimes abnormal samples can still be reconstructed very well.

* They introduce an attention mechanism to propose an attention-based U-Net network to detect anomalies. The network adds an attention module before the skip connection of U-Net network, so that the model pays more attention to the foreground targets.

* The proposed anomaly detection encoder-decoder is implemented by U-Net network with an attention module, and the network structure is shown in Fig. 2. The path on the left side of the network corresponds to the encoder; the path on the right side of the network corresponds to the decoder.

* In the skip connection, the feature map of each resolution in the encoder and the corresponding feature map in the decoder are sent to the attention module , and then the output of the attention module is concatenated with the corresponding feature map in the decoder
 
 
       ![attentionmodel](https://user-images.githubusercontent.com/51711008/231850511-2bd5a0e5-ff28-4320-abae-51c8b8528321.png)
