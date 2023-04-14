
## Key Points

* A deep-learning method named U-Net was applied to improve the skill in forecasting summer (June–August) precipitation for at a one-month lead during the period 1981–2020 in China. The variables of geopotential height,
soil moisture, sea level pressure, sea surface temperature, ocean salinity, and snow were considered as the model input to revise the seasonal prediction of the Climate Forecast System.

* The main structure of the model was the U-Net model (Ronncberger et al., 2015), which is a deep neural network with a fully symmetric encoding–decoding   structure ,The encoder is used for feature compression and the decoder is used to reconstruct features ,Both model inputs and outputs are from a single time point.

* They  divided the coupled dataset into three parts: The training set was used to iteratively optimize the parameters of the model. The validation set was used to verify the eﬀectiveness of the completed training parameters and was not used in the training process. The testing set was used to test the real performance.

* In order to assess the forecast skill as comprehensively as possible, they have used four indices: root-mean-square error (RMSE); anomaly same
sign (AS); temporal correlation coeﬃcient (TCC); and anomaly correlation coeﬃcient (ACC). The RMSE was used to evaluate the Eulerian distance between predictions and observations.
 


images.githubusercontent.com/51711008/231931175-ea17935e-3e2a-4a23-92c6-108dfff4d6db.png)
