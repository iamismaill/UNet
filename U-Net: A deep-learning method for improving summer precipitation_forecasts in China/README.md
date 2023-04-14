
## Key Points

* A deep-learning method named U-Net was applied to improve the skill in forecasting summer (June–August) precipitation for at a one-month lead during the period 1981–2020 in China. The variables of geopotential height,
soil moisture, sea level pressure, sea surface temperature, ocean salinity, and snow were considered as the model input to revise the seasonal prediction of the Climate Forecast System.

* The main structure of the model was the U-Net model (Ronncberger et al., 2015), which is a deep neural network with a fully symmetric encoding–decoding   structure ,The encoder is used for feature compression and the decoder is used to reconstruct features ,Both model inputs and outputs are from a single time point.

* 


They introduce an attention mechanism to propose an attention-based U-Net network to detect anomalies. The network adds an attention module before the skip connection of U-Net network, so that the model pays more attention to the foreground targets.

The proposed anomaly detection encoder-decoder is implemented by U-Net network with an attention module, and the network structure is shown in Fig. 2. The path on the left side of the network corresponds to the encoder; the path on the right side of the network corresponds to the decoder.

In the skip connection, the feature map of each resolution in the encoder and the corresponding feature map in the decoder are sent to the attention module , and then the output of the attention module is concatenated with the corresponding feature map in the decoder![xog](https://user-

images.githubusercontent.com/51711008/231931175-ea17935e-3e2a-4a23-92c6-108dfff4d6db.png)
