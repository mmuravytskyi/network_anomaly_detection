# network_anomaly_detection

## Data preprocessing

## Autoencoder

The purpose of autoencoder is to encode and decode input data. Then error is calculated by compating input data wit autoencoder output.

After teaching process, when error is greater than designated treshold, the sample is classified as anomaly.

### Parameters of our autoencoder

- 10 epoch
- 7 us of processing per sample
- 20% dropout
- Layers dimentions
  - 43
  - 86 - Relu - Overcomplete layer
  - 43
  - 30
  - 20
  - 8
  - 20
  - 30
  - 43 - Sigmoid

First we made autoencoder with 30 epochs but 20 epochs were redundant. They increased learning time but didn't improverd autoencoder precision much.

Overcomplete layer in undercomplete autoencoder allows to check for non obvious connections between samples.

We used Sigmoid as an activation function on the last decoder layer to get normalized results.

## Isolation Forest

## KNN

## Conclusions
