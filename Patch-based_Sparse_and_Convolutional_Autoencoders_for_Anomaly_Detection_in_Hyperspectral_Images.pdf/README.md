## Key Points

The paper proposes a novel non-symmetrical Deep Convolutional Autoencoder (DCAE) for visual anomaly detection. 

* DCAE is optimized to minimize the difference between input and reconstruction for anomaly detection.

* The proposed approach trains a single RotNet as an encoder to generate discriminative representations that are used to train two parallel decoders for image reconstruction.

* The reconstruction errors obtained by the two decoders are combined to produce an anomaly score.

Evaluation Metric

* They use AUROC(Area Under the Receiver Operating Characteristic Curve ) to measure the performance , the Roc curve is created by plotting the true positive rate (TPR) against the false positive rate(FPR.

* Area Under the Receiver Operating Characteristic Curve (AUC-ROC): AUC-ROC is a metric that measures the ability of the anomaly detection model to distinguish between normal and anomalous images 
 
